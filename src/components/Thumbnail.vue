
<template> 
<v-content >
<br>
  <v-row class="mt-4 ml-1" no-gutters>
    <v-col
      v-for="n in 15"
      :key="n"
      class="d-flex child-flex"
      cols="2"
     
    >
      <v-img
        :src="`https://picsum.photos/300/200?image=${n * 5 + 10}`"
        :lazy-src="`https://picsum.photos/6/2?image=${n * 5 + 10}`"
        max-height="125"
        aspect-ratio="1"
        class="grey lighten-2"
      >
        <template v-slot:placeholder>
          <v-row
            class="fill-height ma-0"
            align="center"
            justify="center"
          >
            <v-progress-circular
              indeterminate
              color="grey lighten-5"
            ></v-progress-circular>
          </v-row>
        </template>
      </v-img>
    </v-col>
  </v-row>
  </v-content>
</template>
