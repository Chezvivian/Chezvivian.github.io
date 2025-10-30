---
layout: single
title: "游戏设计"
---

<div style="margin-bottom: 2em;">
  <a href="/podcasts/" style="color: #007acc; text-decoration: none; font-weight: 500;">← 返回 Vivian's 播客小镇</a>
</div>


# Origin（2025-10-30）

对游戏设计的好奇，来自于25级硕士生毕业论文的指导。去年我做了一个游戏本地化主题的翻译认知过程实验，开始对游戏翻译中的各个环节进行思考。正好指导同样感兴趣的硕士学生来做毕业论文的题目。最近在讨论游戏内世界观元素的分类时，我去找了一些游戏设计的文献，发现游戏的类别、叙事方式和交互方式等都有非常大的区别，以至于业界并没有对于游戏叙事方式等有非常固定的分类。而对于译者而言，这既是一个缺失，也是一个可以深挖、研究下去的方向。因为对要翻译、本地化的文本越熟悉，我们越能摸索到解决好本地化问题的核心。

于是就有了这个对游戏设计本身进行学习的频道。我买了一些译著的纸质书，也找到了英文著作的电子版，会一并交给 NotebookLM 来进行学习。接下来，我们就开始吧。


<div class="gd-video" style="margin: 10px 0 18px;">
  <div id="gd-video-mount" style="width: 100%; aspect-ratio: 16 / 9; border: 1px solid #eee; border-radius: 10px; background: #000; display: flex; align-items: center; justify-content: center; color: #9aa7b2; font-size: 0.95rem;">正在加载视频…</div>
  <div style="font-size: 0.9rem; color: #666; margin-top: 6px;">如无法内嵌，请使用备用链接在新窗口打开：
    <a href="https://verbose-temple-e01.notion.site/Game_design-29c5a9c7a666807a94c1dfd5023e065a?source=copy_link" target="_blank" rel="noopener">在 Notion 中观看</a>
  </div>
</div>

<script>
  (function() {
    var NOTION_URL = 'https://verbose-temple-e01.notion.site/Game_design-29c5a9c7a666807a94c1dfd5023e065a?source=copy_link';
    function mountIframe() {
      var mount = document.getElementById('gd-video-mount');
      if (!mount) return;
      // 清空占位并创建 iframe
      mount.innerHTML = '';
      var iframe = document.createElement('iframe');
      iframe.src = NOTION_URL;
      iframe.setAttribute('title', 'Game Design Video');
      iframe.setAttribute('loading', 'lazy');
      iframe.style.width = '100%';
      iframe.style.height = '100%';
      iframe.style.border = '0';
      iframe.style.borderRadius = '10px';
      // 兼容没有 aspect-ratio 的浏览器
      mount.style.position = 'relative';
      if (!('aspectRatio' in document.body.style)) {
        mount.style.paddingTop = '56.25%';
        iframe.style.position = 'absolute';
        iframe.style.top = '0';
        iframe.style.left = '0';
        iframe.style.height = '100%';
      }
      mount.appendChild(iframe);
    }
    function ready(fn){
      if (document.readyState !== 'loading') { fn(); }
      else { document.addEventListener('DOMContentLoaded', fn); }
    }
    ready(function() { mountIframe(); });
  })();
</script>

## Game jargons 游戏行话


<div style="margin: 10px 0 8px;">
  <input id="gjx-filter" type="text" placeholder="搜索术语（中/英/类别）..." style="width:100%; max-width:420px; padding:8px 10px; border:1px solid #dfe6ee; border-radius:6px;" />
</div>

<div id="gjx-list" style="margin: 6px 0 16px;">
  <div style="color:#8aa0b2; font-size:0.95rem;">正在加载术语表…</div>
  <noscript>需要启用 JavaScript 以加载术语表。</noscript>
</div>

<script src="https://cdn.jsdelivr.net/npm/xlsx@0.18.5/dist/xlsx.full.min.js"></script>
<script>
(function(){
  var XLSX_URL = '/files/podcasts/game/游戏行话.xlsx';
  var listEl, filterEl, allItems = [];

  function createItem(termEn, termZh, category){
    var li = document.createElement('li');
    li.style.listStyle = 'none';
    li.style.margin = '8px 0';
    li.style.padding = '0';

    var title = document.createElement('div');
    title.style.fontWeight = 'bold';
    title.textContent = (termZh || '').trim() + (termEn ? ' (' + termEn.trim() + ')' : '');

    var meta = document.createElement('div');
    meta.style.marginTop = '6px';
    meta.style.color = '#444';
    meta.style.background = '#f8f9fb';
    meta.style.borderRadius = '6px';
    meta.style.padding = '8px 12px';
    meta.textContent = (category || '').trim();

    li.appendChild(title);
    if ((category || '').trim()) li.appendChild(meta);
    return li;
  }

  function render(items){
    listEl.innerHTML = '';
    var ul = document.createElement('ul');
    ul.style.listStyle = 'none';
    ul.style.padding = '0';
    items.forEach(function(it){ ul.appendChild(createItem(it.en, it.zh, it.cat)); });
    listEl.appendChild(ul);
  }

  function applyFilter(){
    var q = (filterEl.value || '').toLowerCase().trim();
    if (!q) return render(allItems);
    var filtered = allItems.filter(function(it){
      return (it.en||'').toLowerCase().indexOf(q) > -1 ||
             (it.zh||'').toLowerCase().indexOf(q) > -1 ||
             (it.cat||'').toLowerCase().indexOf(q) > -1;
    });
    render(filtered);
  }

  function normalizeRow(row){
    // 尝试优先匹配列头，否则取前三列
    var keys = Object.keys(row);
    var en = row['English'] || row['english'] || row['EN'] || row['Term'] || row['term'] || row[keys[0]];
    var zh = row['中文'] || row['Chinese'] || row['CN'] || row['译名'] || row['名称'] || row[keys[1]];
    var cat = row['类别'] || row['Category'] || row['用途'] || row['Type'] || row[keys[2]];
    return { en: en ? String(en) : '', zh: zh ? String(zh) : '', cat: cat ? String(cat) : '' };
  }

  function load(){
    listEl = document.getElementById('gjx-list');
    filterEl = document.getElementById('gjx-filter');
  }

  function ready(fn){
    if (document.readyState !== 'loading') fn();
    else document.addEventListener('DOMContentLoaded', fn);
  }

  ready(function(){
    listEl = document.getElementById('gjx-list');
    filterEl = document.getElementById('gjx-filter');
    if (filterEl) filterEl.addEventListener('input', applyFilter);

    // 拉取并解析 xlsx
    fetch(XLSX_URL).then(function(res){ return res.arrayBuffer(); }).then(function(ab){
      var wb = XLSX.read(ab, { type: 'array' });
      var first = wb.SheetNames[0];
      var sheet = wb.Sheets[first];
      var json = XLSX.utils.sheet_to_json(sheet, { raw: false });
      allItems = json.map(normalizeRow).filter(function(it){ return it.en || it.zh; });
      render(allItems);
    }).catch(function(e){
      listEl.innerHTML = '<div style="color:#a33;">术语表加载失败：' + (e && e.message ? e.message : '网络或文件问题') + '</div>';
    });
  });
})();
</script>
