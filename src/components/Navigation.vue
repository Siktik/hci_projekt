<template>
  <nav>
    <ul>
      <li>
        <mail/>
      </li>
      <li>
        <logOut/>
        </li>
        <li>
        <inbox/>
        </li>
        <li>
        <helpCircle/>
      </li>
    </ul>
  </nav>

</template>
<script>

import mail from '@geist-ui/vue-icons/packages/mail'
import logOut from '@geist-ui/vue-icons/packages/log-out'
import inbox from '@geist-ui/vue-icons/packages/inbox'
import helpCircle from '@geist-ui/vue-icons/packages/help-circle'


export default {
name: 'Navigation',
components:{
  mail,
  logOut,
  helpCircle,
  inbox

},

}
</script>
<style>


</style>
