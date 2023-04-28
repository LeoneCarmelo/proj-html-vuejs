<script>
export default {
    name: 'CopyRight',
    props: {
        copyright: String,
        nexgen: String
    }
}
</script>

<template>
    <div class="copyright py-3">
        <div class="container">
            <div class="row">
                <div class="col text-center">
                    <span class="text_grey">{{ copyright }}</span>
                </div>
                <div class="col text-center">
                    <span class="text_grey">&copy; {{ nexgen }}<span
                        class="color_dg">Codings</span>.</span>
                </div>
            </div>
        </div>
    </div>
</template>


<style lang="scss" scoped>
@use '../assets/scss/partials/variables' as *;

   .copyright {
      background: #000;
      position: absolute;
      bottom: 0;
      left: 0;
      width: 100%;

      span {
         font-size: 0.5rem;
      }
   }
.color_dg {
    color: $dark-green
}

.text_grey {
    color: $grey-text
}
</style>