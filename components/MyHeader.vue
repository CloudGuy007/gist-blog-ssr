<template>
  <header class="page-header">
    <div class="container">
      <div class="row">
        <div class="col-md-12">
          <ul class="breadcrumb">
            <li><nuxt-link to="/">{{ $t('HOME.TITLE') }}</nuxt-link></li>
          </ul>
        </div>
      </div>
      <div class="row">
        <div class="col-md-12">
          <h2>{{ $t('HOME.INTRODUCTION') }}</h2>
        </div>
      </div>
    </div>
  </header>
</template>

<style lang="scss">

  .page-header {
    background-color: #35495f;
    border-bottom: 5px solid #3c8070;
    border-top: 5px solid #3c8070;
    margin: 0 0 35px 0;
    min-height: 50px;
    padding: 20px 0;
    position: relative;
    text-align: left;
    .breadcrumb {
      background: none;
      margin: -3px 0 0;
      padding: 0;
      > li {
        text-shadow: none;
      }
      &.breadcrumb-valign-mid {
        position: absolute;
        top: 40%;
        right: 20px;
      }
    }
    h2 {
      border-bottom: 5px solid #3c8070;
      color: #FFF;
      display: inline-block;
      font-weight: 200;
      margin: 0 0 -25px;
      min-height: 37px;
      font-size: 2.6em;
      line-height: 46px;
      padding: 0 0 17px;
      position: relative;
      span {
        color: #999da3;
        display: block;
        font-size: 0.6em;
        font-weight: 300;
        margin: -10px 0 0;
      }
    }
  }

  .page-header-no-title-border h1 {
    border: 0;
  }

  /* Page Header - More Padding */

  .page-header-more-padding {
    padding: 35px 0;
  }

  /* Page Header - Color */

  .page-header-color {
    background-color: #F7F7F7;
    border-bottom: 5px solid #F4F4F4;
    border-top: none;
    h1 {
      border-bottom: none;
      color: #1d2127;
      font-size: 2.3em;
      span {
        opacity: 0.65;
      }
    }
    .breadcrumb > .active {
      opacity: 0.65;
    }
  }

  /* Page Header - Light */

  .page-header-light {
    background-color: #F7F7F7;
    border-bottom: 5px solid #F4F4F4;
    border-top: none;
    h1 {
      border-bottom: none;
      color: #1d2127;
      font-size: 2.3em;
    }
  }

  /* Page Header - Reverse */

  .page-header-reverse {
    text-align: right;
    .breadcrumb {
      float: left;
      left: 20px;
      right: auto;
      margin-top: -10px;
      &.breadcrumb-valign-mid {
        float: left;
        left: 20px;
        right: auto;
        margin-top: -10px;
      }
    }
  }

  /* Page Header - Parallax */

  .page-header.parallax {
    margin: 0 0 35px;
    padding: 180px 0 60px;
  }

  .page-header-center {
    text-align: center;
    .breadcrumb {
      margin: 15px 0 0;
    }
  }

  /* Page Header Custom Background */

  .page-header-custom-background {
    padding: 45px 0;
    background-repeat: repeat;
    background-color: transparent;
    border-top: 0;
    border-bottom: 0;
    h1 {
      color: #FFF;
      border: 0;
      span {
        color: #FFF;
        opacity: 0.7;
      }
    }
    .breadcrumb.breadcrumb-valign-mid {
      top: 36%;
      li.active {
        color: #FFF;
        opacity: 0.7;
      }
      a {
        color: #FFF;
      }
    }
  }

  /* Page Header Custom - Create your Own */

  .page-header.custom-product {
    // background-image: url('./assets/img/custom-header-bg.jpg');
    background-repeat: repeat;
    background-color: #999;
    border-top: 5px solid #888;
    overflow: hidden;
    .row {
      position: relative;
    }
    p.lead {
      color: #E8E8E8;
    }
    img {
      bottom: -47px;
      position: relative;
    }
    h1 {
      color: #FFF;
      margin-bottom: 10px;
      margin-top: 30px;
      border: 0;
    }
  }

  /* Responsive */

  @media (max-width: 991px) {
    .page-header .breadcrumb {
      float: none !important;
      position: static !important;
    }
  }

  @media (max-width: 479px) {
    .page-header {
      padding: 16px 0;
      h1 {
        line-height: 37px;
      }
    }
  }
</style>

