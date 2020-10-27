<template>
    <svg
        width="492"
        height="343"
        viewBox="0 0 492 343"
        fill="none"
        xmlns="http://www.w3.org/2000/svg"
    >
        <path
            d="M149.739 51.1214C155.329 44.638 154.605 34.8507 148.121 29.2609C141.638 23.671 131.851 24.3953 126.261 30.8786L149.739 51.1214ZM16 182.5L4.26085 172.379C-1.08777 178.582 -0.686397 187.876 5.17712 193.596L16 182.5ZM127.177 312.596C133.305 318.573 143.118 318.451 149.096 312.323C155.073 306.195 154.951 296.382 148.823 290.404L127.177 312.596ZM126.261 30.8786L4.26085 172.379L27.7391 192.621L149.739 51.1214L126.261 30.8786ZM5.17712 193.596L127.177 312.596L148.823 290.404L26.8229 171.404L5.17712 193.596Z"
            fill="white"
        />
        <path
            d="M342.261 290.879C336.671 297.362 337.395 307.149 343.879 312.739C350.362 318.329 360.149 317.605 365.739 311.121L342.261 290.879ZM476 159.5L487.739 169.621C493.088 163.418 492.686 154.124 486.823 148.404L476 159.5ZM364.823 29.4043C358.695 23.4269 348.882 23.5491 342.904 29.6771C336.927 35.8051 337.049 45.6184 343.177 51.5957L364.823 29.4043ZM365.739 311.121L487.739 169.621L464.261 149.379L342.261 290.879L365.739 311.121ZM486.823 148.404L364.823 29.4043L343.177 51.5957L465.177 170.596L486.823 148.404Z"
            fill="white"
        />
        <path
            d="M273 16L219 326.5"
            stroke="white"
            stroke-width="31"
            stroke-linecap="round"
            stroke-linejoin="round"
        />
    </svg>
</template>

<script>
export default {};
</script>

<style scoped>
svg {
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    width: 200px;
    height: auto;
    cursor: pointer;
}

svg:hover {
    transition: all 0.3s ease;
}

svg:hover > path:nth-child(1) {
    display: none;
}

svg:hover > path:nth-child(3) {
    transform-origin: center;
    transform: rotate(80deg);
    transition: all 0.3s ease;
}


</style>