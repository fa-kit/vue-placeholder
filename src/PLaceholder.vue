<template>
    <div 
        :style="styles"
        class="placeholder">
    </div>
</template>

<script>
export default {
    props: {
        display: {
            type: String,
            default: 'block'
        },
        maxWidth: {
            type: String,
            default: '100%'
        },
        paddingBottom: String,
        marginBottom: String,
        backgroundColor: {
            type: String,
            default: '#FAFAFA'
        }
    },
    computed: {
        styles() {
            return{
                display: this.display,
                maxWidth: this.maxWidth,
                paddingBottom: this.paddingBottom,
                marginBottom: this.marginBottom,
                backgroundColor: this.backgroundColor,
            }
        },
    }
}
</script>