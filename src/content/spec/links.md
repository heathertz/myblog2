# 友情链接 🔗

欢迎来到友链页面！这里收集了一些优秀的技术博客和实用网站，希望对大家有所帮助。

---

## 🌟 友情博客

<div class="friend-links-grid">

<div class="friend-link-card">
    <a href="https://github.com/ZyPLJ" target="_blank">
        <div class="card-avatar">
            <img src="https://github.githubassets.com/images/modules/logos_page/GitHub-Mark.png" alt="GitHub">
        </div>
        <div class="card-info">
            <h3 class="card-title">GitHub</h3>
            <p class="card-desc">代码托管与开源项目分享</p>
        </div>
    </a>
</div>

</div>

---

## 🛠️ 实用工具

<div class="friend-links-grid">

<div class="friend-link-card">
    <a href="https://ico.pljzy.top" target="_blank">
        <div class="card-avatar">
            <img src="https://ico.pljzy.top/logo.ico" alt="图片转Ico">
        </div>
        <div class="card-info">
            <h3 class="card-title">图片转Ico</h3>
            <p class="card-desc">在线png、jpg、jpeg图片转Ico工具</p>
        </div>
    </a>
</div>

<div class="friend-link-card">
    <a href="https://ebook.deali.cn/" target="_blank">
        <div class="card-avatar">
            <img src="https://ebook.deali.cn/static/favicon.ico" alt="TXT转电子书工具">
        </div>
        <div class="card-info">
            <h3 class="card-title">TXT转电子书工具</h3>
            <p class="card-desc">将TXT文本文件转换为EPUB、MOBI、AZW3等电子书格式</p>
        </div>
    </a>
</div>

</div>

<style>
.friend-links-grid {
    display: grid;
    grid-template-columns: repeat(auto-fill, minmax(320px, 1fr));
    gap: 1.5rem;
    margin: 2rem 0;
}

.friend-link-card {
    background: var(--card-bg);
    border: 1px solid var(--line-divider);
    border-radius: 12px;
    overflow: hidden;
    transition: all 0.3s ease;
    position: relative;
}

.friend-link-card:hover {
    transform: translateY(-4px);
    box-shadow: 0 8px 25px rgba(0, 0, 0, 0.1);
    border-color: var(--primary);
}

.friend-link-card a {
    display: flex;
    align-items: center;
    padding: 0;
    text-decoration: none;
    color: inherit;
    height: 100%;
}

.card-avatar {
    flex-shrink: 0;
    width: 80px;
    height: 80px;
    overflow: hidden;
    display: flex;
    align-items: center;
    justify-content: center;
    border-radius: 12px 0 0 12px;
}

.card-info {
    flex: 1;
    min-width: 0;
    padding: 1rem 1.25rem;
}

.card-avatar img {
    width: 100%;
    height: 100%;
    object-fit: cover;
    transition: transform 0.3s ease;
}

.friend-link-card:hover .card-avatar img {
    transform: scale(1.05);
}

.card-title {
    font-size: 1.1rem;
    font-weight: 600;
    color: var(--text-primary);
    margin: 0 0 0.25rem 0;
    line-height: 1.3;
}

.card-desc {
    font-size: 0.875rem;
    color: var(--text-secondary);
    margin: 0;
    line-height: 1.4;
    display: -webkit-box;
    -webkit-line-clamp: 2;
    -webkit-box-orient: vertical;
    overflow: hidden;
}

.custom-md a:not(.no-styling) {
    margin:0;
    padding:0;
}

/* 响应式设计 */
@media (max-width: 768px) {
    .friend-links-grid {
        grid-template-columns: 1fr;
        gap: 1rem;
    }

    .card-avatar {
        width: 70px;
        height: 70px;
    }

    .card-info {
        padding: 0.875rem 1rem;
    }
}

/* 深色模式优化 */
:root.dark .friend-link-card {
    border-color: var(--line-divider);
}

:root.dark .friend-link-card:hover {
    box-shadow: 0 8px 25px rgba(255, 255, 255, 0.05);
}
</style>
