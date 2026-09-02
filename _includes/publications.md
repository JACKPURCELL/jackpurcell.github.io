<!-- <h2 id="publications" style="margin: 2px 0px -15px;">Recent Publications ([Full List](site._includes.full-publications.md))</h2> -->

## Selected Publications ([Full List](https://scholar.google.com/citations?user=Qsp7ts0AAAAJ))

<style>
/* ---- topic color tokens (light) ---- */
.t-align     { --c-bg:#f2eefc; --c-fg:#6247ba; --c-bd:#e0d6f7; }
.t-redteam   { --c-bg:#fdedf0; --c-fg:#b93e57; --c-bd:#f8d6dd; }
.t-defense   { --c-bg:#ecf6ec; --c-fg:#3f8143; --c-bd:#d4ead6; }
.t-agents    { --c-bg:#e6f6f3; --c-fg:#157c70; --c-bd:#c9ebe5; }
.t-rag       { --c-bg:#fdf4e3; --c-fg:#a2711a; --c-bd:#f5e3c0; }
.t-reasoning { --c-bg:#fdeee4; --c-fg:#b45f28; --c-bd:#f8dcc8; }
.t-serving   { --c-bg:#e6f4fa; --c-fg:#17738f; --c-bd:#c7e6f1; }
.t-watermark { --c-bg:#f9ecf7; --c-fg:#9a3d8c; --c-bd:#f2d8ee; }
.t-bench     { --c-bg:#e9f2fd; --c-fg:#2c6dba; --c-bd:#d0e3f8; }
.t-neutral   { --c-bg:#f2f3f5; --c-fg:#4a5462; --c-bd:#dfe3e8; }

.pub-toolbar {
  display: flex;
  flex-wrap: wrap;
  align-items: baseline;
  gap: 6px;
  margin: 0 0 6px 0;
}
.pub-toolbar-label {
  font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, sans-serif;
  font-size: 0.62rem;
  font-weight: 700;
  letter-spacing: 0.09em;
  text-transform: uppercase;
  color: #9aa3ad;
  /* min-width in rem, not em: em would resolve against this element's own 0.62rem */
  flex: 0 0 auto;
  min-width: 3.6rem;
  padding-right: 4px;
  white-space: nowrap;
}
.pub-filter-btn {
  font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, sans-serif;
  font-size: 0.72rem;
  font-weight: 600;
  line-height: 1.5;
  padding: 3px 10px;
  border-radius: 20px;
  border: 1px solid var(--c-bd);
  background: transparent;
  color: var(--c-fg);
  cursor: pointer;
  transition: background-color .15s ease, color .15s ease, border-color .15s ease, opacity .15s ease;
}
.pub-filter-btn:hover { background: var(--c-bg); }
.pub-filter-btn.is-active {
  background: var(--c-fg);
  border-color: var(--c-fg);
  color: #ffffff;
}
.pub-filter-btn:focus-visible { outline: 2px solid var(--c-fg); outline-offset: 2px; }
.pub-filter-btn.is-empty { opacity: 0.35; }
.pub-filter-btn .pub-count { font-weight: 500; opacity: 0.75; }

.pub-empty {
  font-size: 0.85rem;
  color: #9aa3ad;
  font-style: italic;
  margin: 0 0 18px 0;
}
.pub-empty[hidden] { display: none; }

.pub-list { list-style: none; padding-left: 0; margin: 16px 0 0 0; }
.pub-item { margin: 0 0 18px 0; padding-left: 1.1em; text-indent: -1.1em; }
.pub-item::before { content: "\2022"; padding-right: 0.6em; color: #b3bac2; }
.pub-item.is-hidden { display: none; }
.pub-item .pub-authors,
.pub-item .pub-venue,
.pub-item .pub-badges { display: block; text-indent: 0; padding-left: 1.1em; }
.pub-badges { margin-top: 5px; }
.pub-badge {
  display: inline-block;
  font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, sans-serif;
  font-size: 0.67rem;
  font-weight: 600;
  line-height: 1.7;
  letter-spacing: 0.015em;
  padding: 0 8px;
  margin: 0 4px 3px 0;
  border-radius: 10px;
  border: 1px solid var(--c-bd);
  background: var(--c-bg);
  color: var(--c-fg);
  white-space: nowrap;
  vertical-align: middle;
}
/* the tag the active filter matched reads a shade stronger than its siblings */
.pub-badge.is-matched { background: var(--c-fg); border-color: var(--c-fg); color: #ffffff; }

/* ---- topic color tokens (dark) ---- */
@media (prefers-color-scheme: dark) {
  .t-align     { --c-bg:rgba(150,124,240,0.14); --c-fg:#b3a1f2; --c-bd:rgba(150,124,240,0.32); }
  .t-redteam   { --c-bg:rgba(240,124,150,0.14); --c-fg:#f0a0b1; --c-bd:rgba(240,124,150,0.32); }
  .t-defense   { --c-bg:rgba(110,200,120,0.14); --c-fg:#8ed09a; --c-bd:rgba(110,200,120,0.32); }
  .t-agents    { --c-bg:rgba(80,205,186,0.14);  --c-fg:#6fd3c2; --c-bd:rgba(80,205,186,0.32); }
  .t-rag       { --c-bg:rgba(240,186,90,0.14);  --c-fg:#eec277; --c-bd:rgba(240,186,90,0.32); }
  .t-reasoning { --c-bg:rgba(240,150,95,0.14);  --c-fg:#eda878; --c-bd:rgba(240,150,95,0.32); }
  .t-serving   { --c-bg:rgba(95,190,225,0.14);  --c-fg:#7cc7e4; --c-bd:rgba(95,190,225,0.32); }
  .t-watermark { --c-bg:rgba(220,130,205,0.14); --c-fg:#dfa2d5; --c-bd:rgba(220,130,205,0.32); }
  .t-bench     { --c-bg:rgba(90,170,245,0.14);  --c-fg:#82bcf5; --c-bd:rgba(90,170,245,0.32); }
  .t-neutral   { --c-bg:#2a2c38; --c-fg:#b9bec8; --c-bd:#3b3f4e; }

  .pub-filter-btn.is-active,
  .pub-badge.is-matched { color: #1b1c24; }
  .pub-toolbar-label,
  .pub-empty { color: #7d838f; }
  .pub-item::before { color: #5b606c; }
}
</style>

<div class="pub-toolbar" id="pub-filter-role">
  <span class="pub-toolbar-label">Author</span>
  <button type="button" class="pub-filter-btn t-neutral is-active" data-role="all">All <span class="pub-count"></span></button>
  <button type="button" class="pub-filter-btn t-neutral" data-role="first">First / Co-first <span class="pub-count"></span></button>
  <button type="button" class="pub-filter-btn t-neutral" data-role="co">Co-author <span class="pub-count"></span></button>
</div>

<div class="pub-toolbar" id="pub-filter-topic">
  <span class="pub-toolbar-label">Topic</span>
  <button type="button" class="pub-filter-btn t-neutral is-active" data-topic="all">All <span class="pub-count"></span></button>
  <button type="button" class="pub-filter-btn t-align" data-topic="align">Alignment &amp; Post-Training <span class="pub-count"></span></button>
  <button type="button" class="pub-filter-btn t-redteam" data-topic="redteam">Attacks &amp; Red-Teaming <span class="pub-count"></span></button>
  <button type="button" class="pub-filter-btn t-defense" data-topic="defense">Safety Defense <span class="pub-count"></span></button>
  <button type="button" class="pub-filter-btn t-agents" data-topic="agents">LLM Agents <span class="pub-count"></span></button>
  <button type="button" class="pub-filter-btn t-rag" data-topic="rag">RAG <span class="pub-count"></span></button>
  <button type="button" class="pub-filter-btn t-reasoning" data-topic="reasoning">Reasoning Models <span class="pub-count"></span></button>
  <button type="button" class="pub-filter-btn t-serving" data-topic="serving">LLM Serving <span class="pub-count"></span></button>
  <button type="button" class="pub-filter-btn t-watermark" data-topic="watermark">Watermarking <span class="pub-count"></span></button>
  <button type="button" class="pub-filter-btn t-bench" data-topic="bench">Benchmarking <span class="pub-count"></span></button>
</div>

<p class="pub-empty" id="pub-empty" hidden>No publications match this combination.</p>

<ul class="pub-list">

<li class="pub-item" data-role="first" data-topics="align redteam">
<a href="https://jackpurcell.github.io/assets/ares.pdf">ARES: Adaptive Red-Teaming and End-to-End Repair of Policy-Reward System</a>
<span class="pub-authors"><strong>Jiacheng Liang</strong>, Yao Ma, Tharindu Kumarage, Satyapriya Krishna, Rahul Gupta, Kai-Wei Chang, Aram Galstyan, Charith Peris</span>
<span class="pub-venue">Annual Meeting of the Association for Computational Linguistics (ACL 2026)</span>
<span class="pub-badges"><span class="pub-badge t-align" data-topic="align">Alignment &amp; Post-Training</span><span class="pub-badge t-redteam" data-topic="redteam">Attacks &amp; Red-Teaming</span></span>
</li>

<li class="pub-item" data-role="first" data-topics="reasoning redteam">
<a href="https://jackpurcell.github.io/assets/autoran.pdf">AutoRAN: Weak-to-Strong Jailbreaking of Large Reasoning Models</a>
<span class="pub-authors"><strong>Jiacheng Liang</strong>, Tanqiu Jiang, Yuhui Wang, Rongyi Zhu, Fenglong Ma, Ting Wang</span>
<span class="pub-venue">Annual Meeting of the Association for Computational Linguistics (ACL 2026)</span>
<span class="pub-badges"><span class="pub-badge t-reasoning" data-topic="reasoning">Reasoning Models</span><span class="pub-badge t-redteam" data-topic="redteam">Attacks &amp; Red-Teaming</span></span>
</li>

<li class="pub-item" data-role="first" data-topics="rag redteam">
<a href="https://arxiv.org/pdf/2501.14050">GraphRAG under Fire</a>
<span class="pub-authors"><strong>Jiacheng Liang</strong>, Yuhui Wang, Changjiang Li, Rongyi Zhu, Tanqiu Jiang, Neil Gong, Ting Wang</span>
<span class="pub-venue">IEEE Symposium on Security and Privacy 2026 (IEEE S&amp;P 2026)</span>
<span class="pub-badges"><span class="pub-badge t-rag" data-topic="rag">RAG</span><span class="pub-badge t-redteam" data-topic="redteam">Attacks &amp; Red-Teaming</span></span>
</li>

<li class="pub-item" data-role="co" data-topics="agents redteam bench">
<a href="https://arxiv.org/abs/2602.16901">AgentLAB: Benchmarking LLM Agents against Long-Horizon Attacks</a>
<span class="pub-authors">Tanqiu Jiang, Yuhui Wang, <strong>Jiacheng Liang</strong>, Ting Wang</span>
<span class="pub-venue">International Conference on Machine Learning (ICML 2026)</span>
<span class="pub-badges"><span class="pub-badge t-agents" data-topic="agents">LLM Agents</span><span class="pub-badge t-redteam" data-topic="redteam">Attacks &amp; Red-Teaming</span><span class="pub-badge t-bench" data-topic="bench">Benchmarking</span></span>
</li>

<li class="pub-item" data-role="co" data-topics="agents defense">
<a href="https://arxiv.org/abs/2605.03228">MAGE: Safeguarding LLM Agents against Long-Horizon Threats via Shadow Memory</a>
<span class="pub-authors">Yuhui Wang, Tanqiu Jiang, <strong>Jiacheng Liang</strong>, Charles Fleming, Ting Wang</span>
<span class="pub-venue">ACM Conference on Computer and Communications Security (ACM CCS 2026)</span>
<span class="pub-badges"><span class="pub-badge t-agents" data-topic="agents">LLM Agents</span><span class="pub-badge t-defense" data-topic="defense">Safety Defense</span></span>
</li>

<li class="pub-item" data-role="first" data-topics="align defense">
<a href="https://www.arxiv.org/abs/2602.04448">RASA: Routing-Aware Safety Alignment for Mixture-of-Experts Models</a>
<span class="pub-authors"><strong>Jiacheng Liang</strong>, Yuhui Wang, Tanqiu Jiang, Ting Wang</span>
<span class="pub-venue">Empirical Methods in Natural Language Processing (EMNLP 2026)</span>
<span class="pub-badges"><span class="pub-badge t-align" data-topic="align">Alignment &amp; Post-Training</span><span class="pub-badge t-defense" data-topic="defense">Safety Defense</span></span>
</li>

<li class="pub-item" data-role="first" data-topics="watermark redteam bench">
<a href="https://arxiv.org/pdf/2411.13425">WaterPark: A Robustness Assessment of Language Model Watermarking</a>
<span class="pub-authors"><strong>Jiacheng Liang</strong>, Zian Wang, Lauren Hong, Shouling Ji, Ting Wang</span>
<span class="pub-venue">Empirical Methods in Natural Language Processing (EMNLP 2025)</span>
<span class="pub-badges"><span class="pub-badge t-watermark" data-topic="watermark">Watermarking</span><span class="pub-badge t-redteam" data-topic="redteam">Attacks &amp; Red-Teaming</span><span class="pub-badge t-bench" data-topic="bench">Benchmarking</span></span>
</li>

<li class="pub-item" data-role="first" data-topics="redteam bench">
<a href="https://arxiv.org/pdf/2312.05386">Model Extraction Attacks Revisited</a>
<span class="pub-authors"><strong>Jiacheng Liang</strong>, Ren Pang, Changjiang Li, Ting Wang</span>
<span class="pub-venue">Asia Conference on Computer and Communications Security (Asia CCS 2024)</span>
<span class="pub-badges"><span class="pub-badge t-redteam" data-topic="redteam">Attacks &amp; Red-Teaming</span><span class="pub-badge t-bench" data-topic="bench">Benchmarking</span></span>
</li>

<li class="pub-item" data-role="first" data-topics="align defense">
<a href="https://arxiv.org/pdf/2410.02220">Data to Defense: The Role of Curation in Customizing LLMs Against Jailbreaking Attacks</a>
<span class="pub-authors">Xiaoqun Liu*, <strong>Jiacheng Liang*</strong>, Luoxi Tang, Muchao Ye, Weicheng Ma, Zhaohan Xi</span>
<span class="pub-venue">Empirical Methods in Natural Language Processing (EMNLP 2025)</span>
<span class="pub-badges"><span class="pub-badge t-align" data-topic="align">Alignment &amp; Post-Training</span><span class="pub-badge t-defense" data-topic="defense">Safety Defense</span></span>
</li>

<li class="pub-item" data-role="first" data-topics="serving defense">
<a href="https://arxiv.org/pdf/2608.01718">LaCache: Robust Semantic Caching for LLM Serving</a>
<span class="pub-authors"><strong>Jiacheng Liang</strong>, Yuhui Wang, Tanqiu Jiang, Ting Wang</span>
<span class="pub-badges"><span class="pub-badge t-serving" data-topic="serving">LLM Serving</span><span class="pub-badge t-defense" data-topic="defense">Safety Defense</span></span>
</li>

</ul>

<script>
(function () {
  var roleBar = document.getElementById('pub-filter-role');
  var topicBar = document.getElementById('pub-filter-topic');
  var empty = document.getElementById('pub-empty');
  if (!roleBar || !topicBar) return;

  var items = [].slice.call(document.querySelectorAll('.pub-list .pub-item'));
  var roleButtons = [].slice.call(roleBar.querySelectorAll('.pub-filter-btn'));
  var topicButtons = [].slice.call(topicBar.querySelectorAll('.pub-filter-btn'));
  var role = 'all';
  var topic = 'all';

  // a paper carries several topics, so match against the whole space-separated set
  var topicsOf = {};
  items.forEach(function (item, i) {
    item.setAttribute('data-index', i);
    topicsOf[i] = (item.getAttribute('data-topics') || '').split(/\s+/);
  });

  function matches(item, r, t) {
    var i = item.getAttribute('data-index');
    return (r === 'all' || item.getAttribute('data-role') === r) &&
           (t === 'all' || topicsOf[i].indexOf(t) !== -1);
  }

  function count(r, t) {
    return items.filter(function (item) { return matches(item, r, t); }).length;
  }

  function render() {
    var visible = 0;
    items.forEach(function (item) {
      var show = matches(item, role, topic);
      item.classList.toggle('is-hidden', !show);
      if (show) visible++;
      // highlight whichever of this paper's tags the topic filter selected
      [].forEach.call(item.querySelectorAll('.pub-badge'), function (badge) {
        badge.classList.toggle('is-matched', topic !== 'all' && badge.getAttribute('data-topic') === topic);
      });
    });
    empty.hidden = visible > 0;

    // counts are computed against the other dimension's current selection
    roleButtons.forEach(function (button) {
      var value = button.getAttribute('data-role');
      var n = count(value, topic);
      button.querySelector('.pub-count').textContent = '(' + n + ')';
      button.classList.toggle('is-active', value === role);
      button.classList.toggle('is-empty', n === 0);
    });
    topicButtons.forEach(function (button) {
      var value = button.getAttribute('data-topic');
      var n = count(role, value);
      button.querySelector('.pub-count').textContent = '(' + n + ')';
      button.classList.toggle('is-active', value === topic);
      button.classList.toggle('is-empty', n === 0);
    });
  }

  roleBar.addEventListener('click', function (event) {
    var button = event.target.closest('.pub-filter-btn');
    if (!button) return;
    role = button.getAttribute('data-role');
    render();
  });

  topicBar.addEventListener('click', function (event) {
    var button = event.target.closest('.pub-filter-btn');
    if (!button) return;
    topic = button.getAttribute('data-topic');
    render();
  });

  render();
})();
</script>
