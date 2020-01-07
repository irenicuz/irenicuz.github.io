<template>
    <header>
        <nav>
            <ul>
                <li>
                    <nuxt-link to="/">Home</nuxt-link>
                </li>
                <li>
                    <nuxt-link to="/blog">Blog</nuxt-link>
                </li>
                <li>
                    <nuxt-link to="/song">Song of the moment</nuxt-link>
                </li>
                <li>
                    <nuxt-link to="/interests">Things I like</nuxt-link>
                </li>
            </ul>
        </nav>
    </header>
</template>

<style lang="scss" scoped>
    header {
        display: flex;
        margin-left: auto;
        margin-right: auto;
        max-width: 960px;

        h1 {
            font-weight: 400;
        }

        a {
            padding: 10px 30px;
            text-decoration: none;
            display: inline-block;
        }

        ul {
            list-style: none;
            padding: 10px;
            display: flex;

            li {
                font-size: 22px;
                transition: background-color 1s;
                font-weight: 300;
                font-family: 'Source Sans Pro', sans-serif;

                &:hover {
                    background-color: #f3f3f3;
                }

                &:first-child {
                    border-top-left-radius: 8px;
                    border-bottom-left-radius: 8px;
                }

                &:last-child {
                    border-top-right-radius: 8px;
                    border-bottom-right-radius: 8px;
                }
            }
        }

        @media screen and (max-width: 700px){ 

            nav {

                width: 100%;

                ul {
                    flex-direction: column;

                    li {
                        border-radius: 8px;
                        background-color: #f3f3f3;
                        margin-bottom: 5px;

                        a {
                            width: 100%;
                        }

                        &:last-child {
                            margin-bottom: 0;
                        }
                        
                    }
                }
                
            }
        }
    }
</style>