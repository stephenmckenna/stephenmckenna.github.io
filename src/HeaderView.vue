
<script>
import { fabGithub, fabLinkedin } from '@quasar/extras/fontawesome-v6';
import { ref, defineComponent } from 'vue'
import AboutView from './AboutView.vue'
import ExperienceView from './ExperienceView.vue'
import ProjectsView from './ProjectsView.vue'

  export default {
    components: {
      AboutView,
      ExperienceView,
      ProjectsView
    },
    setup() {
      return {
        tab: ref('about')
      }
    },
    created() {
      this.fabGithub = fabGithub;
      this.fabLinkedin = fabLinkedin;
    }
  }
</script>

<template>
  <q-layout style='overflow-y: auto;' view="hhh lpr fff">
    <q-header style='position: sticky' class="bg-accent text-white q-ma-lg rounded-borders q-pt-md q-px-md">
      <q-toolbar>
        <div class="left q-mt-lg" style="display: inline-flex; flex-direction: column;">
          <q-toolbar-title class="text-h2">
            Stephen McKenna
          </q-toolbar-title>
          <q-toolbar-title class="text-h5 q-pl-none">
          Software Engineer
          </q-toolbar-title>
        </div>
        <div class="absolute-right q-py-lg" style="display: inline-flex; flex-direction: column; justify-content:center; text-align: right; width: fit-content">
          <p class="text-subtitle1 q-my-xs">Pittsburgh, PA</p>
          <a class="text-subtitle1 contactLinks" href='tel:724-553-9400' style='text-decoration:none;'>(724) 553-9400</a>
          <a class="text-subtitle1 contactLinks" href='mailto:mckennask00@gmail.com' style='text-decoration: none;'>mckennask00@gmail.com</a>
          <div style="width: 100%; display: flex; flex-direction: row; justify-content: end;">
            <a class="q-mx-sm contactLinks" target="_blank" href="https://github.com/stephenmckenna" style='height: 25px; width: 25px;'>
              <q-icon class="q-mx-sm q-mt-sm" href="github.com/stephenmckenna" :name="fabGithub" style="height: 25px; width: 25px;"/>
            </a>
            <a class="q-mx-sm contactLinks" target="_blank" href="https://www.linkedin.com/in/-stephenmckenna/" style='height: 25px; width: 25px;'>
              <q-icon class="q-mx-sm q-mt-sm" :name="fabLinkedin" style="height: 25px; width: 25px;"/>
            </a>
          </div>
        </div>
      </q-toolbar>

      <q-tabs align="center" v-model="tab">
        <q-tab name="about" label="About Me" />
        <q-tab name="experience" label="Experience" />
        <q-tab name="projects" label="Projects" />
      </q-tabs>
    </q-header>
    <q-page-container style='padding-top: 0px'>
      <q-tab-panels v-model="tab" animated style="color: #5f5f5f;" class="bg-secondary q-ma-lg rounded-borders q-pt-md q-px-md">
        <q-tab-panel name="about">
          <AboutView/>
        </q-tab-panel>
        <q-tab-panel name="experience">
          <ExperienceView/>
        </q-tab-panel>
        <q-tab-panel name="projects">
          <ProjectsView/>
        </q-tab-panel>
      </q-tab-panels>
    </q-page-container>
    <div style='height: 50px'/>
  </q-layout>
</template>
