<template>
    <svg
        width="375"
        height="111"
        viewBox="0 0 375 111"
        fill="none"
        xmlns="http://www.w3.org/2000/svg"
    >
        <path
            d="M35.688 3.05599C47.24 3.05599 57.2213 5.23466 65.632 9.59199C74.144 13.848 80.6293 19.9787 85.088 27.984C89.648 35.9893 91.928 45.4133 91.928 56.256C91.928 67.0987 89.648 76.5227 85.088 84.528C80.6293 92.432 74.144 98.512 65.632 102.768C57.2213 106.923 47.24 109 35.688 109H2.70398V3.05599H35.688ZM35.688 97.6C49.368 97.6 59.8053 94.0027 67 86.808C74.1946 79.512 77.792 69.328 77.792 56.256C77.792 43.0827 74.144 32.7973 66.848 25.4C59.6533 18.0027 49.2666 14.304 35.688 14.304H16.536V97.6H35.688Z"
            stroke="white"
            stroke-width="4"
        />
        <path
            d="M172.797 85.44H126.589L118.077 109H103.485L141.789 3.66399H157.749L195.901 109H181.309L172.797 85.44ZM168.845 74.192L149.693 20.688L130.541 74.192H168.845Z"
            stroke="white"
            stroke-width="4"
        />
        <path
            d="M300.147 3.05599L260.171 109H244.211L204.235 3.05599H218.979L252.267 94.408L285.555 3.05599H300.147Z"
            stroke="white"
            stroke-width="4"
        />
        <path
            d="M329.145 14.304V49.72H367.753V61.12H329.145V97.6H372.313V109H315.313V2.90399H372.313V14.304H329.145Z"
            stroke="white"
            stroke-width="4"
        />
    </svg>
</template>

<script>
export default {
    mounted() {
        let timeIncrease = 0
        const paths = this.$el.querySelectorAll("svg > path")
        paths.forEach(path => {
            let finish = path.getTotalLength()
            path.style.strokeDasharray = finish
            path.style.strokeDashoffset = finish

            path.style.animation = `strokeAnimation 2s ease`
            timeIncrease += 0.3
            console.log(timeIncrease)
        })
    },
    beforeMount() {
      console.log("updated")
    }
};
</script>

<style scoped>
svg {
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
}

@keyframes strokeAnimation {
    to {
        stroke-dashoffset: 0px;
    }
}

</style>