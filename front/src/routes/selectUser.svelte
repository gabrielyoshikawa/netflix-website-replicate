<script>
    import Profile from "../components/profile.svelte";
    import ButtonSelectUser from "../components/buttonSelectUser.svelte";

    let userInformation = [
        { userImage: "src/assets/user-image-blue.png", userName: "User 1" },
        { userImage: "src/assets/user-image-green.png", userName: "User 2" },
        { userImage: "src/assets/user-image-red.png", userName: "User 3" },
        { userImage: "src/assets/add-profile.png", userName: "Add Profile" },
    ];
</script>

<div class="content">
    <div class="box">
        <div class="ttl">
            <p>Who's watching?</p>
        </div>
        <div class="profiles">
            {#each userInformation as boxInformation}
                <Profile
                    userImage={boxInformation.userImage}
                    userName={boxInformation.userName}
                />
            {/each}
        </div>
        <div class="manage-options">
            <ButtonSelectUser />
        </div>
        
    </div>
</div>

<style>
    .content {
        width: 100vw;
        height: 100vh;
        background-color: #141414;
        display: flex;
        justify-content: center;
        align-items: center;
    }

    .box {
        width: 45%;
        height: 60%;
        display: flex;
        flex-direction: column;
        justify-content: space-around;
    }

    .ttl {
        width: 100%;
        height: 20%;
        display: flex;
        justify-content: center;
        align-items: center;
    }

    .profiles {
        width: 100%;
        height: 50%;
        display: flex;
    }

    .manage-options {
        width: 100%;
        height: 20%;
        display: flex;
        justify-content: center;
        align-items: end;
    }

    .ttl p {
        font-size: 2rem;
        color: white;
        font-weight: 500;
        font-family: Sans, Helvetica Neue, Segoe UI, Roboto, Ubuntu, sans-serif;
    }
</style>
