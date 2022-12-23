---
page: true
date: 2021-06-30
title: page_4
sidebar: true
---
<script setup>
import Page from "../.vitepress/theme/components/Page.vue";
import { useData } from "vitepress";
const { theme } = useData();
const pageSize = theme.value.pageSize;
const posts = theme.value.posts.slice(9,12)
</script>
<Page :posts="posts" :pageCurrent="4" :pagesNum="11" />