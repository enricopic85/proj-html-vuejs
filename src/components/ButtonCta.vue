<template>
   <div class="cta">
        Get started today
    </div>
</template>

<script>
export default {
    
}
</script>

<style lang="scss" scoped>
@import '@/../style/variables.scss';
    .cta{
                color: $white;
                background-color: $jungle-green-v;
                width: 150px;
                height: 40px;
                line-height: 40px;
                font-size: 12px;
                text-align: center;
                border-radius: 2px;
                cursor: pointer;
                &:hover{
                    background-color: $klein-blue;
                }
            }
</style>