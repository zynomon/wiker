<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>{{ page.title }}</title>
  <meta name="description" content="{{ page.description }}">
  <meta property="og:title"        content="{{ page.title }}">
  <meta property="og:description"  content="{{ page.description }}">
  <meta property="og:image"        content="{{ '/assets/thumb.png' | relative_url }}">
  <meta property="og:image:width"  content="1200">
  <meta property="og:image:height" content="630">
  <meta property="og:type"         content="website">
  <meta property="og:url"          content="{{ page.url | absolute_url }}">
  <meta property="og:site_name"    content="{{ site.title }}">
  <meta name="twitter:card"        content="summary_large_image">
  <meta name="twitter:title"       content="{{ page.title }}">
  <meta name="twitter:description" content="{{ page.description }}">
  <meta name="twitter:image"       content="{{ '/assets/thumb.png' | relative_url }}">
  <meta name="theme-color"         content="{{ page.color }}">
  <meta property="og:image:alt"    content="{{ page.title }}">
  <meta name="twitter:image:alt"   content="{{ page.title }}">

  {% if page.icon %}
  <link rel="icon" type="image/svg+xml" href="{{ '/icons/' | append: page.icon | relative_url }}">
  {% endif %}

  <script>
    (function(){
      try {
        var t = localStorage.getItem('theme');
        if (t) document.documentElement.setAttribute('data-theme', t);
        else if (window.matchMedia('(prefers-color-scheme: light)').matches)
          document.documentElement.setAttribute('data-theme', 'light');
      } catch(e){}
    })();
  </script>

  <link rel="stylesheet" href="{{ '/assets/css/style.css' | relative_url }}">
</head>
<body>

{% if page.bg %}
<div class="page-bg" aria-hidden="true">
  <img src="{{ page.bg | relative_url }}" alt="">
</div>
{% endif %}

<div class="frame">

  <header id="site-header">

    <div class="header-band">
      {% if site.header_bg %}
      <img src="{{ site.header_bg | relative_url }}" class="header-band-img" alt="" aria-hidden="true">
      {% endif %}

      {% if site.header_logo %}
      <img src="{{ site.header_logo | relative_url }}" class="header-logo" alt="{{ site.title }}">
      {% else %}
      <span class="header-wordmark">{{ site.title }}</span>
      {% endif %}

      <span class="header-path" aria-hidden="true">{{ page.url }}</span>

      <div class="header-controls">
        <button class="ctrl-btn" id="ctrl-theme" aria-label="toggle theme">
          <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" aria-hidden="true"><circle cx="12" cy="12" r="5"/><line x1="12" y1="1" x2="12" y2="3"/><line x1="12" y1="21" x2="12" y2="23"/><line x1="4.22" y1="4.22" x2="5.64" y2="5.64"/><line x1="18.36" y1="18.36" x2="19.78" y2="19.78"/><line x1="1" y1="12" x2="3" y2="12"/><line x1="21" y1="12" x2="23" y2="12"/><line x1="4.22" y1="19.78" x2="5.64" y2="18.36"/><line x1="18.36" y1="5.64" x2="19.78" y2="4.22"/></svg>
        </button>
        <button class="ctrl-btn" id="ctrl-pin" aria-label="pin header">
          <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" aria-hidden="true"><line x1="12" y1="17" x2="12" y2="22"/><path d="M5 17h14v-1.76a2 2 0 0 0-1.11-1.79l-1.78-.9A2 2 0 0 1 15 10.76V6h1a2 2 0 0 0 0-4H8a2 2 0 0 0 0 4h1v4.76a2 2 0 0 1-1.11 1.79l-1.78.9A2 2 0 0 0 5 15.24Z"/></svg>
        </button>
      </div>
    </div>

    {% if page.nav_links or site.nav_links %}
    {% assign _nav = page.nav_links | default: site.nav_links %}
    <nav class="header-nav" aria-label="site navigation">
      {% for item in _nav %}
      <a href="{{ item.url }}"
         {% if item.url contains 'http' %}target="_blank" rel="noopener noreferrer"{% endif %}
         {% if page.url == item.url %}aria-current="page"{% endif %}>
        {% if item.icon %}<img src="{{ item.icon | relative_url }}" class="nav-icon" alt="" aria-hidden="true">{% endif %}
        {{ item.label }}
      </a>
      {% endfor %}
    </nav>
    {% endif %}

  </header>

  <main>
    {{ content }}
  </main>

  <footer>

    <hr>
    <div class="footer-row">

      {% if site.footer_logo %}
      <img src="{{ site.footer_logo | relative_url }}" class="footer-logo" alt="{{ site.title }}">
      {% endif %}

      {% if site.footer_links %}
      <div class="footer-links">
        {% for item in site.footer_links %}
        <a href="{{ item.url }}"
           {% if item.url contains 'http' %}target="_blank" rel="noopener noreferrer"{% endif %}>
          {{ item.label }}
        </a>
        {% endfor %}
      </div>
      {% endif %}
    </div>
  </footer>

</div>

<script>
(function () {
  var R      = document.documentElement;
  var hdr    = document.getElementById('site-header');
  var pinBtn = document.getElementById('ctrl-pin');
  var thmBtn = document.getElementById('ctrl-theme');

  if (!hdr) return;

  function store(k, v) { try { localStorage.setItem(k, v); } catch(e){} }
  function recall(k)   { try { return localStorage.getItem(k); } catch(e){ return null; } }

  var pinned = recall('pin') === '1';
  if (pinned) hdr.classList.add('is-pinned');

  if (pinBtn) {
    if (pinned) pinBtn.classList.add('is-active');
    pinBtn.addEventListener('click', function () {
      pinned = !pinned;
      hdr.classList.toggle('is-pinned', pinned);
      pinBtn.classList.toggle('is-active', pinned);
      store('pin', pinned ? '1' : '0');
    });
  }

  if (thmBtn) {
    thmBtn.addEventListener('click', function () {
      var next = R.getAttribute('data-theme') === 'light' ? 'dark' : 'light';
      R.setAttribute('data-theme', next);
      store('theme', next);
    });
  }

  var tick = false;
  window.addEventListener('scroll', function () {
    if (tick) return;
    tick = true;
    requestAnimationFrame(function () {
      hdr.classList.toggle('is-scrolled', window.scrollY > 40);
      tick = false;
    });
  }, { passive: true });

  document.querySelectorAll('.header-nav a').forEach(function (a) {
    var icon = a.querySelector('.nav-icon');
    if (!icon) return;

    a.addEventListener('mouseenter', function () {
      icon.style.transition = 'opacity 0.15s ease, transform 0.15s ease';
      icon.style.opacity    = '1';
      icon.style.transform  = 'scale(1) translateY(0)';
    });

    a.addEventListener('mousemove', function (e) {
      var r  = a.getBoundingClientRect();
      var mx = (e.clientX - r.left) / r.width  - 0.5;
      var my = (e.clientY - r.top)  / r.height - 0.5;

      icon.style.transition = 'opacity 0.15s ease';
      icon.style.transform  = 'perspective(400px) rotateX(' + (-my * 20) + 'deg) rotateY(' + (mx * 20) + 'deg) scale(1.1)';
    });

    a.addEventListener('mouseleave', function () {
      icon.style.transition = 'opacity 0.15s ease, transform 0.15s ease';
      icon.style.opacity    = '0';
      icon.style.transform  = 'scale(0.7) translateY(4px)';
    });
  });

  var COPY  = '<svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><rect x="9" y="9" width="13" height="13" rx="2"/><path d="M5 15H4a2 2 0 0 1-2-2V4a2 2 0 0 1 2-2h9a2 2 0 0 1 2 2v1"/></svg>';
  var CHECK = '<svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><polyline points="20 6 9 17 4 12"/></svg>';

  document.querySelectorAll('pre code').forEach(function (c) {
    var pre = c.parentElement;
    if (pre.parentElement.classList.contains('code-wrap')) return;
    var wrap = document.createElement('div');
    wrap.className = 'code-wrap';
    pre.parentNode.insertBefore(wrap, pre);
    wrap.appendChild(pre);
    var btn = document.createElement('button');
    btn.className = 'code-copy';
    btn.setAttribute('aria-label', 'copy code');
    btn.innerHTML = COPY;
    btn.addEventListener('click', function () {
      if (!navigator.clipboard) return;
      navigator.clipboard.writeText(c.textContent).then(function () {
        btn.innerHTML = CHECK;
        btn.classList.add('did-copy');
        setTimeout(function () {
          btn.innerHTML = COPY;
          btn.classList.remove('did-copy');
        }, 2000);
      }).catch(function () {});
    });
    wrap.appendChild(btn);
  });

})();
</script>

</body>
</html>