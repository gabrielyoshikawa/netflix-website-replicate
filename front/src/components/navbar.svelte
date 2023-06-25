<script>
    import NavbarCategories from "./navbarCategories.svelte";

    let categoriesOptions = [
        { categories: "Home" },
        { categories: "TV Shows" },
        { categories: "Movies" },
        { categories: "New & Popular" },
        { categories: "My List" },
        { categories: "Browse by Languages" },
    ];

    function changeNavbarColor() {
        let navbar = document.getElementById("navbar");
        let scrollPosition = window.pageYOffset || document.documentElement.scrollTop;

        if (scrollPosition > 10) navbar.style.backgroundColor = "black";
        else navbar.style.backgroundColor = "rgba(0, 0, 0, 0.24)";

    }

    window.addEventListener("scroll", changeNavbarColor);
</script>

<nav class="navbar" id="navbar">
    <div class="categoriesSpace">
        <a href="/">
            <img src="src/assets/netflix-logo.png" alt="Netflix logo" />
        </a>
        <div class="categoriesResponsiveBox">
            {#each categoriesOptions as categoryOptions}
                <NavbarCategories categories={categoryOptions.categories} />
            {/each}
        </div>
    </div>
    <div class="iconsSpace">
        <i class="fas fa-search" />
        <i class="far fa-bell" />
        <img src="src/assets/user-image-blue.png" alt="User profile icon" />
        <i class="fas fa-caret-down" />
    </div>
</nav>

<style>
    nav {
        width: 100%;
        height: 9%;
        max-height: 70px;
        display: flex;
        justify-content: space-evenly;
        position: fixed;
        top: 0;
        z-index: 1;
        transition: 1.5s;
        background-color: rgba(0, 0, 0, 0.24);
    }

    .categoriesSpace {
        width: 70%;
        display: flex;
        align-items: center;
        justify-content: space-between;
    }

    .categoriesSpace a {
        width: 15%;
        height: 100%;
        display: flex;
    }

    .categoriesResponsiveBox {
        width: 100%;
        height: 100%;
        display: flex;
        align-items: center;
        justify-content: start;
    }

    .iconsSpace {
        width: 20%;
        display: flex;
        align-items: center;
        justify-content: end;
    }

    .iconsSpace img {
        min-width: 35px;
        max-width: 35px;
        min-height: 35px;
        max-height: 35px;
        margin-right: 1em;
        border-radius: 10%;
    }

    i {
        font-size: 1.2rem;
        margin-right: 1em;
        color: white;
    }
</style>
