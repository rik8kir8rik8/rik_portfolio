<template>
    <div id="skills">
        <h1>Skills</h1>
        <h2>Language</h2>
        <skilltable title="C#" subtitle="★★★" text=".Net FreameWork"/>
        <skilltable title="VB" subtitle="★★" text=".Net FreameWork"/>
        <skilltable title="JS" subtitle="★★★" text="Vue.js"/>
        <skilltable title="PHP" subtitle="★" text="Lumen,Larabel"/>
        <h2>Touls</h2>
        <skilltable title="Ai" subtitle="★★★" text=".Net FreameWork"/>
        <skilltable title="Ps" subtitle="★★★" text=".Net FreameWork"/>
    </div>

</template>

<script>
import skilltable from './skilltable.vue'

export default {
  name: 'skills',
  components: {
      skilltable
  }
}
</script>

<style>
#skills{
    height:45rem;
    margin-bottom:20rem;
}
</style>

