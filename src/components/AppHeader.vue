<script>

import AppLogo from './AppLogo.vue';
import AppNav from './AppNav.vue';
import JumboHeader from './JumboHeader.vue';

export default {
    name: 'AppHeader',
    components: {
        AppLogo,
        AppNav,
        JumboHeader
    }
}
</script>

<!-- html -->
<template>
    <header>
        <div class="container">
            <div>
                <AppLogo />
            </div>
            <div>
                <AppNav />
            </div>
        </div>
        <div class="jumbo">
            <JumboHeader/>

        </div>
    </header>
</template>


<style lang="scss" scoped>
.container {
    display: flex;
    justify-content: space-between;
    align-items: center;
}
</style>