<template>
  <header id="header">
    <div class="flex flex-wrap w-4/5 mx-auto">
      <div class="flex py-2">
        <Logo></Logo>
      </div>
      <div class="flex py-6 ml-auto">
        <ul class="flex flex-wrap items-center justify-end">
          <li class="link min-w-full md:min-w-0">
            <a href="/docs/v0.3">
              <span class="font-semibold mr-1">Documentation</span>
            </a>
          </li>
          <li class="link min-w-full md:min-w-0">
            <ProjectDropdown></ProjectDropdown>
          </li>
          <li class="link min-w-full md:min-w-0">
            <CommunityDropdown></CommunityDropdown>
          </li>
        </ul>
      </div>
    </div>
  </header>
</template>

<script>
import Logo from '~/components/Logo.vue'
import ProjectDropdown from '~/components/ProjectDropdown.vue'
import CommunityDropdown from '~/components/CommunityDropdown.vue'

export default {
  name: 'Header',
  components: {
    Logo,
    ProjectDropdown,
    CommunityDropdown
  }
}
</script>

<style scoped>
li {
  margin-left: 1.25rem;
}
</style>
