<template>
    <div id="uswdsHeader">
        <div class="usa-overlay"></div>
        <header class="usa-header usa-header--basic" role="banner">
            <div class="usa-nav-container">
                <div class="usa-navbar">
                    <div class="usa-logo" id="basic-logo">
                        <em class="usa-logo__text"><a href="/" title="Home" aria-label="Home">{{ title }}</a></em>
                    </div>
                    <button class="usa-menu-btn">Menu</button>
                </div>
                <nav role="navigation" class="usa-nav">
                    <button class="usa-nav__close"><img src="~uswds/src/img/close.svg" alt="close"></button>
                    <ul class="usa-nav__primary usa-accordion"><li class="usa-nav__primary-item">
                        <button class="usa-accordion__button usa-nav__link  usa-current" aria-expanded="false" aria-controls="basic-nav-section-one"><span>Current section</span></button>
                        <ul id="basic-nav-section-one" class="usa-nav__submenu"><li class="usa-nav__submenu-item">
                            <a href="#">Navigation link</a>
                        </li><li class="usa-nav__submenu-item">
                            <a href="#">Navigation link</a>
                        </li><li class="usa-nav__submenu-item">
                            <a href="#">Navigation link</a>
                        </li></ul></li><li class="usa-nav__primary-item">
                        <button class="usa-accordion__button usa-nav__link" aria-expanded="false" aria-controls="basic-nav-section-two"><span>Section</span></button>
                        <ul id="basic-nav-section-two" class="usa-nav__submenu"><li class="usa-nav__submenu-item">
                            <a href="#">Navigation link</a>
                        </li><li class="usa-nav__submenu-item">
                            <a href="#">Navigation link</a>
                        </li><li class="usa-nav__submenu-item">
                            <a href="#">Navigation link</a>
                        </li></ul></li><li class="usa-nav__primary-item">
                        <a class="usa-nav__link" href="javascript:void(0)"><span>Simple link</span></a>
                    </li></ul><form class="usa-search usa-search--small ">
                    <div role="search">
                        <label class="usa-sr-only" for="basic-search-field-small">Search small</label>
                        <input class="usa-input" id="basic-search-field-small" type="search" name="search">
                        <button class="usa-button" type="submit"><span class="usa-sr-only">Search</span></button>
                    </div>
                </form>
                </nav>
            </div>
        </header>


        <div class="usa-overlay"></div>
        <main id="main-content"></main>
    </div>
</template>

<script>
    export default {
        name: 'HeaderUSWDS',
        props: {
            title: {
                type: String,
                default: 'Add your title in App.vue or hide this with CSS'
            }
        }
    }
</script>

<style  scoped lang="sass">
    @import '~uswds/dist/css/uswds.css'
</style>