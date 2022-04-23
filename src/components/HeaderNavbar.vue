<template>
  <nav class="navbar navbar-expand-md navbar-light greenA">
    <div class="container-fluid">
      <h4 class="px-2">
        <span class="fw-light fs-4">NPO法人&ensp;</span>
        <span class="fs-3">あまちゃんの会</span>
      </h4>
      <button
        class="navbar-toggler"
        type="button"
        data-bs-toggle="collapse"
        data-bs-target="#navbarSupportedContent"
        aria-controls="navbarSupportedContent"
        aria-expanded="false"
        aria-label="Toggle navigation"
      >
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse" id="navbarSupportedContent">
        <ul class="navbar-nav me-auto mb-2 mb-lg-0">
          <div v-for="item in menuContents" :key="item.text">
            <li class="nav-item">
              <div
                class="nav-link active px-2 mx-1 my-auto text-primary fs-4"
                aria-current="page"
                type="button"
                @click="item.func"
              >
                {{ item.text }}
              </div>
            </li>
          </div>
        </ul>
      </div>
    </div>
  </nav>
</template>

<script lang="ts">
import { defineComponent, PropType } from "vue";
import router from "@/router";
export interface Menu {
  text: string;
  func: void;
}

export default defineComponent({
  name: "HeaderComponent",
  props: {
    menuContents: {
      type: Array as PropType<Menu[]>,
      default: () => [
        { text: "トップ", func: () => router.push({ name: "HomeView" }) },
        { text: "活動", func: () => router.push({ name: "AboutView" }) },
      ],
    },
  },
});
</script>
