<template>
    <div id="skills">
        <h1>Skills</h1>
        <h2>Languages</h2>
        <skilltable title="C#" subtitle="★★★" text=".NET FreameWork"/>
        <skilltable title="VB" subtitle="★★" text=".NET FreameWork"/>
        <skilltable title="JS" subtitle="★★★" text="Vue.js"/>
        <skilltable title="PHP" subtitle="★" text="Lumen,Laravel"/>
        <h2>Tools</h2>
        <skilltable title="Ai" subtitle="★★★" text="Adobe Illustrator CS6"/>
        <skilltable title="Ps" subtitle="★★★" text="Adobe Photoshop CS6"/>
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

