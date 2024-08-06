<template>
  <div
    class='offcanvas offcanvas-start'
    data-bs-scroll='true'
    tabindex='-1'
    id='file'
  >
    <div class='offcanvas-header'>
      <h5 class='offcanvas-title'>Backdrop with scrolling</h5>
      <button
        type='button'
        class='btn-close'
        data-bs-dismiss='offcanvas'
        aria-label='Close'
      ></button>
    </div>
    <div class='offcanvas-body'>
      <p>Try scrolling the rest of the page to see this option in action.</p>
    </div>
  </div>
</template>
<script>
export default {
  name: 'FileMenu'
}
</script>