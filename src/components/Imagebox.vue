<template>
  <div class="image-box-container">
    <div class="close-btn">
        <img src="https://d29fhpw069ctt2.cloudfront.net/icon/image/39219/preview.png" alt="">
    </div>

    <div class="image-viewer">
        <img class="image-showed" src="https://s3.ap-southeast-1.amazonaws.com/okxe.2019/products/361/208361/208361_69826_left_20210630023114_2P1X8mOT_l.jpg" alt="">

        <div class="btn-left">
            <img src="https://image.flaticon.com/icons/png/512/507/507257.png" alt="">
        </div>
        <div class="btn-right">
            <img src="https://image.flaticon.com/icons/png/512/271/271226.png" alt="">
        </div>
    </div>

    <div class="total-image-container">
        <div class="total-image-container">
            <span class="current-image">6</span> / <span class="total-image">12</span>
        </div>
    </div>

    <div class="others-image-container">
        <div class="others-image">
            <div class="image-item">
                <img src="https://s3.ap-southeast-1.amazonaws.com/okxe.2019/products/361/208361/208361_69826_left_20210630023114_2P1X8mOT_l.jpg" alt="">
            </div>
            <div class="image-item">
                <img src="https://s3.ap-southeast-1.amazonaws.com/okxe.2019/products/361/208361/208361_69826_left_20210630023114_2P1X8mOT_l.jpg" alt="">
            </div>
            <div class="image-item">
                <img src="https://s3.ap-southeast-1.amazonaws.com/okxe.2019/products/361/208361/208361_69826_left_20210630023114_2P1X8mOT_l.jpg" alt="">
            </div>
            <div class="image-item">
                <img src="https://s3.ap-southeast-1.amazonaws.com/okxe.2019/products/361/208361/208361_69826_left_20210630023114_2P1X8mOT_l.jpg" alt="">
            </div>
            <div class="image-item">
                <img src="https://s3.ap-southeast-1.amazonaws.com/okxe.2019/products/361/208361/208361_69826_left_20210630023114_2P1X8mOT_l.jpg" alt="">
            </div>
            <div class="image-item">
                <img src="https://s3.ap-southeast-1.amazonaws.com/okxe.2019/products/361/208361/208361_69826_left_20210630023114_2P1X8mOT_l.jpg" alt="">
            </div>
            <div class="image-item">
                <img src="https://s3.ap-southeast-1.amazonaws.com/okxe.2019/products/361/208361/208361_69826_left_20210630023114_2P1X8mOT_l.jpg" alt="">
            </div>
            <div class="image-item">
                <img src="https://s3.ap-southeast-1.amazonaws.com/okxe.2019/products/361/208361/208361_69826_left_20210630023114_2P1X8mOT_l.jpg" alt="">
            </div>
            <div class="image-item">
                <img src="https://s3.ap-southeast-1.amazonaws.com/okxe.2019/products/361/208361/208361_69826_left_20210630023114_2P1X8mOT_l.jpg" alt="">
            </div>
            <div class="image-item">
                <img src="https://s3.ap-southeast-1.amazonaws.com/okxe.2019/products/361/208361/208361_69826_left_20210630023114_2P1X8mOT_l.jpg" alt="">
            </div>
            <div class="image-item">
                <img src="https://s3.ap-southeast-1.amazonaws.com/okxe.2019/products/361/208361/208361_69826_left_20210630023114_2P1X8mOT_l.jpg" alt="">
            </div>
        </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Imagebox",
  components: {},
};
</script>

<style lang="scss" scoped>
.image-box-container {
    max-width: 720px;
    height: 100vh;
    // background-color: rgba(25,25,25,.7);
    background-color: black;
    margin: auto;
    overflow: hidden;

    .close-btn {
        width: 28px;
        height: 28px;
        margin-top: 32px;
        margin-left: 16px;
        background-color: white;
        border-radius: 50%;

        > img {
            width: 100%;
            height: 100%;
        }

        &:hover {
            cursor: pointer;
        }
    }

    .image-viewer {
        position: relative;
        margin-top: 16px;
        padding: 0px 20px;
        height: 75vh;

        > .image-showed {
            width: 100%;
            height: 100%;
        }

        > .btn-left, .btn-right {
            position: absolute;
            width: 40px;
            height: 40px;
            background-color: rgba(25,25,25,.4);
            border-radius: 50%;

            &:hover {
                cursor: pointer;
            }

            > img {
                width: 100%;
                height: 100%;
            }
        }

        > .btn-left {
            left: 24px;
            top: 50%;
        }

        > .btn-right {
            right: 24px;
            top: 50%;
        }
    }

    .total-image-container {
        margin: 24px 0px;

        .total-image-container {
            margin: auto;
            width: 56px;
            // height: 24px;
            text-align: center;
            color: white;
            font-size: 14px;
            padding: 2px 13px;
            border-radius: 50%;
            background-color: #222222;
            border-top-left-radius: 50px 50px;
            border-bottom-left-radius: 50px 50px;
            border-top-right-radius: 50px 50px;
            border-bottom-right-radius: 50px 50px;
        }
    }

    .others-image-container {
        padding: 0px 20px;
        text-align: center;

        .others-image {
            white-space: nowrap;
            overflow-x: auto;
            width: 100%;
        }
        
        .image-item {
            width: 56px;
            height: 56px;
            margin-right: 8px;
            display: inline-block;

            img {
                width: 100%;
                height: 100%;
            }
        }
    }

    /* Custom scroll bar */
    /* width */
    ::-webkit-scrollbar {
        height: 6px;
    }

    /* Track */
    ::-webkit-scrollbar-track {
        background: #f1f1f1; 
    }
    
    /* Handle */
    ::-webkit-scrollbar-thumb {
        background: #888; 
    }

    /* Handle on hover */
    ::-webkit-scrollbar-thumb:hover {
        background: #555; 
    }
}

</style>