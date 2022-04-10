<template>
  <div class="container">
    <p class="fs-2 p-2 text-center">概要</p>
    <div class="card">
      <div class="card-body">
        <h5 class="card-title fs-4">主な活動内容</h5>
        <div class="card-text fs-5">
          <div class="py-1">✓ 地域の施設訪問、レクリエーション</div>
          <div class="py-1">✓ 認知症カフェ</div>
          <div class="py-1">✓ あま市民病院でのボランティア</div>
        </div>
      </div>
      <div class="text-center">
        <img
          src="../assets/RAUL_VALDES.jpg"
          class="img-fluid rounded"
          alt="ImageHere"
        />
      </div>
    </div>
    <div class="p-2">
      <table class="table table-borderless bg-info rounded">
        <tbody>
          <tr>
            <th class="fs-5">受賞歴</th>
          </tr>
          <tr>
            <td class="fs-6">地域○○ 内閣総理大臣賞 20○○年</td>
          </tr>
        </tbody>
      </table>
    </div>
    <div class="p-2">
      <div class="p-1 fs-5">協力NPO</div>
      <ul class="list-group fs-6">
        <li class="list-group-item">傾聴の会</li>
        <li class="list-group-item">わくわくもりあげ隊</li>
      </ul>
    </div>
    <div class="px-2 py-4 my-4 fs-6 rounded-3 bg-light">
      <p class="fst-italic">ボランティアを一緒にしませんか？</p>
      <p class="fst-italic">
        あまちゃんの会に、ボランティアの依頼をしませんか？
      </p>
      <div class="pt-1">連絡先</div>
      <table class="table table-bordered">
        <tbody>
          <tr>
            <th>代表</th>
            <td>渡辺みづえ</td>
          </tr>
          <tr>
            <th>電話</th>
            <td>000-000-0000</td>
          </tr>
          <tr>
            <th>事務局メール</th>
            <td>aaa@bbb.com</td>
          </tr>
        </tbody>
      </table>
    </div>
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";

export default defineComponent({
  name: "HomeView",
});
</script>
