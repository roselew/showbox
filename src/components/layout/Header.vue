<template>
    <a-layout-header class="header">

        <img src="../../assets/logo.svg">
        <a-input-search class="header__search" enter-button placeholder="Szukaj"/>
        <a-dropdown>
            <a class="ant-dropdown-link" @click="e => e.preventDefault()">
                <a-avatar :size="32" icon="user" />
            </a>
            <a-menu slot="overlay">
                <a-menu-item>
                    <span><a-icon type="user" /> Konto</span>
                </a-menu-item>
                <a-menu-item>
                    <span><a-icon type="file-add" /> Dodaj szablon</span>
                </a-menu-item>
                <a-menu-divider />
                <a-menu-item>
                    <span><a-icon type="logout" /> Wyloguj</span>
                </a-menu-item>
            </a-menu>
        </a-dropdown>
        

    </a-layout-header>
</template>

<script>
export default {
    
}
</script>

<style lang="less">

    .header {
        display: flex;
        justify-content: space-between;
        align-items: center;
        padding: 0px 24px;
        background-color: @gray-2;
        border-bottom: solid 1px #303030;

        &__search {
            width: 320px;
            background-color: @gray-1;
        }

    }
</style>