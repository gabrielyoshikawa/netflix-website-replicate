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

    const navbar = document.querySelector(".navbar");
    window.onscroll = () => {
        console.log(window.scrollY)
        if (window.scrollY > 10) {
            navbar.classList.add("nav-active");
        } else {
            navbar.classList.remove("nav-active");
        }
    };
</script>

<nav class="navbar">
    <div class="categoriesSpace">
        <img src="src/assets/netflix-logo.png" alt="Netflix logo" />
        {#each categoriesOptions as categoryOptions}
            <NavbarCategories categories={categoryOptions.categories} />
        {/each}
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
        height: 10%;
        background-color: red;
        display: flex;
        justify-content: center;
        position: fixed;
        top: 0;
    }

    /* .navbar {
        width: 100%;
        position: fixed;
        transition: 0.3s ease-in-out;
    } */

    .nav-active {
        background-color: #fff;
        box-shadow: 5px -1px 12px -5px grey;
    }

    .categoriesSpace {
        width: 55%;
        background-color: lightpink;
        display: flex;
        align-items: center;
        justify-content: space-between;
    }

    .categoriesSpace img {
        width: 15%;
        height: 100%;
    }

    .iconsSpace {
        width: 39%;
        background-color: lightblue;
        display: flex;
        align-items: center;
        justify-content: end;
    }

    .iconsSpace img {
        width: 7%;
        height: 55%;
        margin-right: 0.7em;
        border-radius: 10%;
    }

    i {
        font-size: 1.2rem;
        margin-right: 1em;
        color: white;
    }
</style>
