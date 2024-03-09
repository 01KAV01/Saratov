<nav>
    <div class="nav-container">
    <a href="/" class="nav-logo" title="Back to Homepage">На главную</a>
        <div class="nav-links">
        {#each nav as link}
            <a href={link.href} class="link">{link.title}</a>
        {/each}
        </div>
    </div>
</nav>

    <div class="container">

    <slot></slot>
    </div>
    <script>
        const nav = [
        {
        title:'История',
        href:'/about',
        },

        {
        title:'Достопримечательности',
        href:'/blog',
        },

        {
        title:'Галлерея',
        href:'/project',
        },

        
    ]
        </script>
    <style>
    .container {
    max-width: 1400px;
    margin: 50px auto;
    }
    </style>