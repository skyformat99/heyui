<template>
  <div class="doc">
    <h2>Upload</h2>
    <p>HeyUI's upload will provide a set of styles and provide seven cattle upload demo.</p>
    <p>Different systems can be developed based on their upload implementation.</p>
    <p>All of the examples will be used with <a href="https://github.com/moxiecode/plupload" target="_blank">plupload</a>, because the component has already implemented drag and drop and upload functions, and it will not be expanded here.</p>
    <p>We will provide a demo using the plupload qiniu upload. Because everyone implements the uploaded package are not consistent, so here will provide a <span class="link" @click="goDown">example</span>。</p>

    <p class="component-name-tip">In non-string templates，it is necessary to use <code>h-upload</code>. </p>

    <h3>Single image upload-file object</h3>
    <example demo="dataplugins/uploader1"></example>
  
    <h3>Multiple image upload - array of file objects</h3>
    <p>Add the limit parameter to limit the total number of uploads</p>
    <example demo="dataplugins/uploader2"></example>

    <h3>Single image upload - url</h3>    
    <example demo="dataplugins/uploader3"></example>

  
    <h3>Multiple image upload - url array</h3>
    <example demo="dataplugins/uploader4"></example>

    <h3>Single file upload</h3>
    <example demo="dataplugins/uploader5"></example>
  
    <h3>Multi-file upload</h3>
    <example demo="dataplugins/uploader6"></example>

  
    <h3>Drag and drop upload</h3>
    <example demo="dataplugins/uploader7"></example>


    <h3>Uploader Property</h3>
    <table class="table">
      <tr>
        <th>Property</th>
        <th>Description</th>
        <th>Type</th>
        <th>Optional</th>
        <th>Default</th>
      </tr>
      <tr>
        <td>type</td>
        <td>File or picture presentation mode</td>
        <td>String</td>
        <td>file, image, files, images</td>
        <td>file</td>
      </tr>
      <tr>
        <td>dataType</td>
        <td>The data model of the file object or url</td>
        <td>String</td>
        <td>file, url</td>
        <td>file</td>
      </tr>
      <tr>
        <td>uploadList</td>
        <td>Uploading list</td>
        <td>Array</td>
        <td>-</td>
        <td>-</td>
      </tr>
      <tr>
        <td>files</td>
        <td>List of files that have been uploaded successfully</td>
        <td>Array</td>
        <td>-</td>
        <td>-</td>
      </tr>
      <tr>
        <td>className</td>
        <td>Custom class name</td>
        <td>String</td>
        <td>-</td>
        <td>-</td>
      </tr>
    </table>

    <h3 class="democodes">General examples of qiniu</h3>
    <p>This example shows the general processing plan. If you use another upload method, please refer to the file modification. <a href="https://github.com/heyui/heyui/blob/master/doc/components/demos/common/qiniu.vue" target="_blank">example</a></p>
    <codes src="/common/qiniu.vue" type="html"></codes>
  </div>
</template>

<script>

export default {
  data () {
    return {
    }
  },
  methods: {
    goDown() {
      this.$ScrollIntoView(this.$el.querySelector('.democodes'), {
        align: {
          top: 0,
          topOffset: 80
        }
      });
    }
  }
}
</script>