<script>
export default {
    data() {
        return {
            headerLinks: [
                {
                    name: 'CHARACTERS',
                    url: '#',
                    active: false,
                },
                {
                    name: 'COMICS',
                    url: '#',
                    active: true,
                },
                {
                    name: 'MOVIES',
                    url: '#',
                    active: false,
                },
                {
                    name: 'TV',
                    url: '#',
                    active: false,
                },
                {
                    name: 'GAMES',
                    url: '#',
                    active: false,
                },
                {
                    name: 'COLLECTIBLES',
                    url: '#',
                    active: false,
                },
                {
                    name: 'VIDEOS',
                    url: '#',
                    active: false,
                },
                {
                    name: 'FANS',
                    url: '#',
                    active: false,
                },
                {
                    name: 'NEWS',
                    url: '#',
                    active: false,
                },
                {
                    name: 'SHOP',
                    url: '#',
                    active: false,
                },
            ],
        }
    },

}
</script>

<template>
    <header class="container">
        <nav>
            <figure><img src="../assets/img/dc-logo.png" alt="Logo DC"></figure>
            <ul>
                <li v-for="item in headerLinks" :key="index" :class="item.active ? 'active' : ''">
                    {{ item.name }}
                </li>
            </ul>
        </nav>
    </header>
</template>

<style lang="scss" scoped>
@use '../style/partials/variables' as *;

header {
    width: 100%;
}

nav {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 1rem 0;

    img {
        width: 80%;
    }

    ul {
        display: flex;
        width: 60%;

        li {
            margin-right: 1.5rem;
            font-weight: bolder;
            color: $dc-gray;
        }

        li.active {
            color: $dc-blue;
        }
    }
}
</style>