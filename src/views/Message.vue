<template>
  <div>
    <b-sidebar id="sidebar-no-header" aria-labelledby="sidebar-no-header-title" no-header shadow visible="true">
      <template #default="{ hide }">
        <div class="p-3">
          <h4 id="sidebar-no-header-title">Custom header sidebar</h4>
          <p>
            Cras mattis consectetur purus sit amet fermentum. Cras justo odio, dapibus ac facilisis
            in, egestas eget quam. Morbi leo risus, porta ac consectetur ac, vestibulum at eros.
          </p>
          <nav class="mb-3">
            <b-nav vertical>
              <b-nav-item active @click="hide">Active</b-nav-item>
              <b-nav-item href="#link-1" @click="hide">Link</b-nav-item>
              <b-nav-item href="#link-2" @click="hide">Another Link</b-nav-item>
            </b-nav>
          </nav>
          <b-button variant="primary" block @click="hide">Close Sidebar</b-button>
        </div>
      </template>
    </b-sidebar>

    <b-navbar type="light" variant="light">
      <b-nav-form>
        <b-form-input class="mr-sm-2" placeholder="Search"></b-form-input>
        <b-button variant="outline-success" class="my-2 my-sm-0" type="submit">Search</b-button>
      </b-nav-form>
    </b-navbar>

    <b-navbar type="dark" variant="info" fixed="bottom">
      <!--        <div style="background-color: yellow; width: 100%">
              </div>-->
      <b-form-textarea rows="3"
                       max-rows="6" placeholder="메시지를.."></b-form-textarea>
      <b-button size="sm" class="my-2 my-sm-0" type="submit">전송</b-button>

    </b-navbar>
<!--    <section>section...</section>-->

  </div>
</template>

<script>
export default {
  name: "Message",

  created() {
    // document.body.style.
  }
};
</script>

<style scoped>
/*header {
  position: fixed;
  top: 0; left: 300px;
}*/
</style>
