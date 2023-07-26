<template>
  <footer class="footer footer_bg">
    <div class="container">
      <div class="row">
        <FooterContacts />
        <FooterNavigation :footerMenuClients="footerMenuClients" />
        <FooterClient :footerMenuClient="footerMenuClient" />
        <FooterIcons />
      </div>
    </div>
  </footer>
</template>

<script>
import { menuList, menuClient,menuClients } from '../../constants/menuLinks'
import FooterIcons from './FooterIcons'
import FooterNavigation from './FooterNavigation'
import FooterClient from './FooterClient'
 import FooterContacts from './FooterContacts'
export default {
  data() {
    return {
      footerMenu: menuList,
      footerMenuClient: menuClient,
      footerMenuClients: menuClients,
    }
  },
  components: {
    FooterIcons,
    FooterNavigation,
    FooterClient,
     FooterContacts,
  },
}
</script>