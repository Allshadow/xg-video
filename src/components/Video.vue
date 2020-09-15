<template>
    <div ref="videoId"></div>
</template>

<script>
    import HlsPlayer from 'xgplayer-hls';

    export default {
        name: 'HelloWorld',
        created() {
        },
        mounted() {
            this.initVideo();

        },
        data() {
            return {}
        },
        components: {},
        methods: {
            //官网地址
            //http://h5player.bytedance.com/gettingStarted/
            initVideo() {
                let player = new HlsPlayer({
                    el: this.$refs.videoId,
                    url: 'http://ivi.bupt.edu.cn/hls/cctv1hd.m3u8'
                });
            }
        }
    }
</script>

<style scoped>

</style>
