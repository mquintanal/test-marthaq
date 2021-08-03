<template>
<v-app>
    <template>
        <div>
            <v-app-bar app clipped-left clipped-right color="black" dense dark>
                <v-toolbar-title class="align-center d-flex">
                    <span class="logo-icon">
                        <img src="@/assets/images/logo.png" />
                    </span>
                    <span class="logo-text ml-2">
                    </span>
                </v-toolbar-title>
                <v-toolbar-items class="hidden-xs-only">
                    <v-btn flat v-for="item in menuItems" :key="item.title">
                        {{ item.title }}
                    </v-btn>
                </v-toolbar-items>
                <v-spacer></v-spacer>
                <v-btn icon>
                    <v-icon>mdi-magnify</v-icon>
                </v-btn>
                <v-btn icon>
                    <v-icon>mdi-bell</v-icon>
                </v-btn>
                <img src="@/assets/images/account.png">
                <v-btn icon>
                    <v-icon>mdi-menu-down</v-icon>
                </v-btn>
            </v-app-bar>
        </div>
    </template>

</v-app>
</template>

<script>

export default {
    name: 'App',

    components: {
    },

    data: () => ({
        menuItems: [{ title: 'Home'},
            {title: 'TV Shows'},
            {title: 'Movies'},
            {title: 'New & Popular'},
            {title: 'My List'}
        ]
    }),
};
</script>
