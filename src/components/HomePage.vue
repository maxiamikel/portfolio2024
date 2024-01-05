<template>
    <div class="home-page">
        <img 
            src="../assets/fondo.png"
             alt=""
             class="home-page__image"
        >
        <div class="home-page__content">
            <img 
                src="../assets/foto.jpeg" 
                alt=""
                class="home-page__content__image"
            >
            <p class="home-page__content__name">La gata largona</p>
            <div class="home-page__content_repport">
                <div class="home-page__content_repport__items">
                    <p class="home-page__content_repport__items__number">1.2</p>
                    <p class="home-page__content_repport__items__text">Texto item</p>
                </div>
                <div class="home-page__content_repport__items">
                    <p class="home-page__content_repport__items__number">19</p>
                    <p class="home-page__content_repport__items__text">Projetos</p>
                </div>
                <div class="home-page__content_repport__items">
                    <p class="home-page__content_repport__items__number">7</p>
                    <p class="home-page__content_repport__items__text">Experiencias profesional</p>
                </div>
            </div>
            <div class="home-page__content_control">
                <button class="home-page__content_control__button">Conectar</button>
                <button class="home-page__content_control__button celeste">Ver más</button>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name:"HomePage"
}
</script>

<style lang="scss" scoped>
    .home-page{
        border: solid 1px;
        width: 100%;
        height: 400px;
        position: relative;
        &__image{
            width: 100%;
            height: 100%;
            position: absolute;
            top: 0px;
            left: 0px;
        }
        &__content{
            border: solid 1px;
            position: absolute;
            top: 0px;
            left: 0px;
            width: 100%;
            height: 100%;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            &__image{
                width: 100px;
                height: 100px;
                border-radius: 50%;
            }
            &__name{
                color: #fff;
                font-weight: bold;
                font-size: 17px;
                margin-bottom: 0px;
            }
            &_repport{
                display: flex;
                justify-content:space-around;
                align-items: center;
                text-align: center;
                border-top: solid 1px #fff;
                margin-top: 0px;
                &__items{
                    color: #ffffff;
                    width: 100px;
                    height: 100px;
                    &__number{
                        color:#d4ab16;
                        font-weight: bold;
                    }
                    &__text{
                        font-size: 14px;
                    }
                }
            }
            &_control{
                display: flex;
                justify-content: space-around;
                padding: 10px;
                &__button{
                    background: rgb(7, 63, 7);
                    border: none;
                    padding: 5px 12px 5px 12px;
                    margin: 5px;
                    color: #fff;
                    border-radius: 6px;
                    width: 100px;
                    &.celeste{
                        background: #3498db;
                    }
                }
            }
        }
    }
</style>