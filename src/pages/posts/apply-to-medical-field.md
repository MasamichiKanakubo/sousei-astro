---
title: "医療分野への応用例"
pubDate: "2024-07-09"
slug: "apply-to-medical-field"
description: "電子カルテのユーザビリティ"
hero: "/images/medical-header.png"
tags: ["medical"]
layout: "../../layouts/BlogPostLayout.astro"
---

<!DOCTYPE html>
<html lang="ja">

<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <meta name="theme-color" content="#5588CC">
  <!-- タイトルは書き換えること -->
  <title>認知工学研究紹介のページ</title>
  <!-- CSSファイルやJavaScriptファイルを読み込む-->
  <!-- ここから -->
  <link rel="stylesheet" href="./css/takao/style.css">
  <!-- ここまで -->
  <!--ここからCSS---------------------------------->
  <style>
    body {
      display: flex;
      height: 100vh;
      flex-direction: column;
      font-family: system-ui, -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
    }
    .content {
      display: flex;
      flex: 1;
    }
    .main {
      flex: 1;
      padding: 20px;
    }
    .sawarabi-mincho-regular {
      font-family: "Sawarabi Mincho", serif;
      font-weight: 400;
      font-style: normal;
    }
    .hospital {
      background-image: url("https://www.tottori-med.jrc.or.jp/trch/wp-content/uploads/2020/06/4023f48dfe10585327bb1d4a9c24f5b1.jpg");
      background-size: cover;
      opacity: 70%;
    }
    h2.medical-record {
      border-left: 6px solid rgba(255, 166, 181, 0.75);
      border-bottom: 2px solid rgb(255, 166, 181);
      padding-left: 0.6rem;
      background-color: rgb(241, 163, 255, 0.15);
      margin-top: 2rem;
      margin-left: 0.5rem;
      font-size: 24px;
      padding-top: 0.5rem;
    }
    .container-1 {
      margin-top: 1.5rem;
      display: flex;
      align-items: center;
      justify-content: space-between;
      background-color: #fff;
      padding: 20px;
      border-radius: 10px;
      box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
      width: 100%;
      max-width: 1200px;
    }
    .text-1 {
      flex: 1;
    }
    .modal-target {
      flex: 1;
      display: flex;
      justify-content: flex-end;
    }
    .modal-target img {
      max-width: 60%;
      height: auto;
      border-radius: 10px;
    }
    .modal-dialog {
      position: fixed;
      top: 0;
      left: 0;
      right: 0;
      bottom: 0;
      background-color: hsla(0, 100%, 0%, 0.3);
      overflow: hidden;
      user-select: none;
      display: grid;
      place-items: center;
    }
    body:has(.modal-dialog) {
      overflow: hidden;
    }
    .modal-dialog img {
      object-fit: contain;
    }
    h5.bottom-border {
      border-bottom: 3px solid gray;
      margin-left: 1rem;
      padding-left: 0.5rem;
      margin-top: 2rem;
    }
    h2.surgery {
      border-left: 6px solid rgba(255, 166, 181, 0.75);
      border-bottom: 2px solid rgb(255, 166, 181);
      padding-left: 0.6rem;
      background-color: rgb(241, 163, 255, 0.15);
      margin-top: 2rem;
      margin-left: 0.5rem;
      font-size: 24px;
      padding-top: 0.5rem;
    }
    .footer {
      margin-top: 1rem;
      background-color: rgba(171, 167, 172, 0.15);
      text-align: center;
    }
    .hover-text {
      display: none;
      /*初期状態で非表示にする*/
      position: absolute;
      /*親要素に対して絶対配置にする*/
      background-color: rgba(0, 0, 0, 0.5);
      color: white;
      padding: 5px;
      border-radius: 5px;
      z-index: 1;
      top: 5%;
    }
  </style>
  <link href="https://maxcdn.bootstrapcdn.com/bootstrap/4.5.2/css/bootstrap.min.css" rel="stylesheet">
  <script src="https://cdn.jsdelivr.net/npm/vue@2.6.12"></script>
</head>

<body>
  <div class="container">
    <div class="hospital">
    </div>
    <h2 class="medical-record">電子カルテのユーザビリティ</h2>
    <div class="record1">電子カルテの使いやすさを向上させるためのインターフェースデザイン研究</div>
    <p></p>
    <h5 class="bottom-border">
      ユーザビリティとは
    </h5>
    <div class="text">利用者が機械やコンピュータを
      <span style="background-color: yellow;">
        不自由なく使えるように考慮</span>
      した設計のことである．
    </div>
    <style>
      .text {
        margin-top: 1rem;
      }
      .highlight {
        background-color: rgb(255, 255, 0);
        color: red;
      }
  </style>
    <div class="accordion">
      <div class="accordion-header">1. 学習容易性</div>
      <div class="accordion-content">
        <p>使用するシステムが、利用者にとってわかりやすく、今までの経験から推測できて、使用法を学ぶ時間をあまりかけずにすぐ使えるかどうか。利用者が技術を習得するまでの時間は、利用者の労力を消費していることにつながる。</p>
      </div>
    </div>
    <div class="accordion">
      <div class="accordion-header">2. 効率性</div>
      <div class="accordion-content">
        <p>使用方法を一度学習したら、高い生産性が達成され維持できるかどうか。システムの反応時間などにも依存する。</p>
      </div>
    </div>
    <div class="accordion">
      <div class="accordion-header">3. 記憶しやすさ</div>
      <div class="accordion-content">
        <p>まれにしか使用しない利用者にも、使用法をすぐに思い出せるかどうか。もう一度学びなおすことなく、使えるかどうか
          。
        </p>
      </div>
    </div>
    <div class="accordion">
      <div class="accordion-header">4. エラー</div>
      <div class="accordion-content">
        <p>システムそのもののエラーの発生頻度が少なく、致命的なエラーが起きないように設計されているかどうか。もしエラーが発生しても、容易に回復できるかどうか。</p>
      </div>
    </div>
    <div class="accordion">
      <div class="accordion-header">5. 満足感</div>
      <div class="accordion-content">
        <p>利用者が心地よく使用でき、積極的に使用したいと思えるかどうか。</p>
      </div>
    </div>
    <style>
      .accordion {
        background-color: #fff;
        border: 1px solid #ddd;
        border-radius: 5px;
        margin: 10px 0;
        overflow: hidden;
        box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
        transition: box-shadow 0.3s ease;
      }
      .accordion:hover {
        box-shadow: 0 6px 8px rgba(0, 0, 0, 0.15);
      }
      .accordion-header {
        cursor: pointer;
        padding: 10px;
        text-align: left;
        font-size: 16px;
        border: none;
        outline: none;
        transition: background-color 0.3s, padding 0.3s;
        display: flex;
        align-items: center;
        justify-content: space-between;
      }
      .accordion-header:hover,
      .accordion-header.active {
        background-color: rgb(255, 100, 255, 0.15);
      }
      .accordion-header::after {
        content: "\032C";
        font-size: 20px;
        transition: transform 0.3s;
      }
      .accordion-header.active::after {
        transform: rotate(540deg);
        /* Rotate to create an 'X' */
      }
      .accordion-content {
        background-color: white;
        max-height: 0;
        overflow: hidden;
        padding: 0 15px;
        transition: max-height 0.3s ease, padding 0.3s ease;
      }
      .accordion-content p {
        margin: 15px 0;
      }
      .accordion-content.show {
        max-height: 200px;
        /* Adjust as needed */
        padding: 15px;
      }
   </style>
    の５つに分類することができる．
    <div class="container-1">
      <div class="text-1">
        <h5><span style="border-bottom: 2px solid brown;">ユーザビリティ評価</span></h5>
        <p>医師や看護師を対象にした電子カルテの使いやすさに関する調査研究. ユーザビリティテストやインタビューを通じて, 現行システムの問題点を洗い出し, 改善策を提案する．
          <br>
        <p class="text-2"></p>
        </p>
      </div>
      <div class="modal-target">
        <img src="https://ferret-one.akamaized.net/images/6193821c0431b1121450550d/original.jpeg?utime=1637057052"
          alt="説明画像">
      </div>
    </div>
    <div class="container-1">
      <div class="text-1">
        <h5><span style="border-bottom: 2px solid brown;">患者ポータルの設計の評価</span></h5>
        <p>患者が自分の医療情報を閲覧し, 健康管理に役立てるためのポータルサイトの設計とその効果を評価する研究. ユーザーエクスペリエンスの観点から評価</p>
      </div>
      <div class="modal-target">
        <img src="https://medibase.cloud/wp-content/uploads/2022/03/image2-3.jpg" alt="説明画像">
      </div>
    </div>
    <h2 class="surgery">臨床意思決定支援システム</h2>
    <div class="text">医療従事者は患者に対して，迅速かつ的確な診断や治療法を決断しなければならないが，これには
      <span style="color: red;">
        かなりの負担</span>
      がかかる．
      <p>診療にAIやビッグデータを使用することで, 過去のデータなどから速やかに決断を下し, 医療従事者を支援システムがある．</p>
    </div>
    <div class="container-1">
      <div class="text-1">
        <h5><span style="border-bottom: 2px solid brown;">CDSSやNEWS</span></h5>
        <p>ビッグデータを活用し、サーベイランス(調査)システムやバイタルサイン(生命兆候)を点数化することで、急変リスクを判定できる</p>
      </div>
      <div class="modal-target">
        <img
          src="https://be-nurse.com/wp-content/uploads/2016/08/%E6%84%8F%E6%80%9D%E6%B1%BA%E5%AE%9A%E6%94%AF%E6%8F%B4%E3%81%A8%E3%81%AF.jpg"
          alt="説明画像">
      </div>
    </div>
    <h2 class="surgery">医療情報の標準化</h2>
    <p>異なる医療機関やシステム間で情報を共有しやすくし, 医療の質を向上させるための重要な取り組みである．患者の診療記録，検査結果，処方情報などの医療データが一貫性を持ち，解釈や交換が容易になることを目指す．</p>
    <style>
      table {
        width: 100%;
        border-collapse: collapse;
        margin-top: 1.5rem;
      }
      th,
      td {
        border: 1px solid #ddd;
        padding: 8px;
        text-align: left;
      }
      th {
        background-color: #F2F2F2;
      }
      tr:nth-child(even) {
        background-color: #F9F9F9;
      }
      tr:hover {
        background-color: #F1F1F1;
      }
    </style>
    </head>
    <body>
      <h5 class="bottom-border">医療標準化に期待されるメリット</h5>
      <table>
        <tr>
          <th></th>
          <th>効果(メリット)</th>
        </tr>
        <tr>
          <td>国民</td>
          <td>・スマホ等で自らの医療情報を把握でき持ち運び可能<br>・通院を要せず，タイムリーに検査結果等を把握できる</td>
        </tr>
        <tr>
          <td>医療機関</td>
          <td>・より正確な患者への問診を効率的に実施<br>
            ・他の医療機関の診療情報提供書等の取り込み作業が不要<br>・データの二次利用へ貢献</td>
        </tr>
        <tr>
          <td>保険者</td>
          <td>・重複検査の防止<br>・医療費の適正化</td>
        </tr>
        <tr>
          <td>ベンダー</td>
          <td>・計画的かつ効率的なシステム開発が可能<br>・カスタムオーダー対応からの解放</td>
        </tr>
      </table>
  </div>
  <script src="https://code.jquery.com/jquery-3.5.1.slim.min.js"></script>
  <script src="https://cdn.jsdelivr.net/npm/@popperjs/core@2.5.4/dist/umd/popper.min.js"></script>
  <script src="https://maxcdn.bootstrapcdn.com/bootstrap/4.5.2/js/bootstrap.min.js"></script>
  <script>
    document.addEventListener('DOMContentLoaded', function () {
      var acc = document.getElementsByClassName("accordion-header");
      for (var i = 0; i < acc.length; i++) {
        acc[i].addEventListener("click", function () {
          this.classList.toggle("active");
          var content = this.nextElementSibling;
          if (content.classList.contains("show")) {
            content.classList.remove("show");
          } else {
            var allContents = document.getElementsByClassName("accordion-content");
            for (var j = 0; j < allContents.length; j++) {
              allContents[j].classList.remove("show");
            }
            content.classList.add("show");
          }
        });
      }
    });
  </script>
</body>

</html>
