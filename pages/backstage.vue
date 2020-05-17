<template>
  <div>
    <div id="test-editor">
      <textarea style="display:none;">### 关于 Editor.md
**Editor.md** 是一款开源的、可嵌入的 Markdown 在线编辑器（组件），基于 CodeMirror、jQuery 和 Marked 构建。
    </textarea>
    </div>
  </div>
</template>

<script>
import $ from "jquery";
import editormd from "editor.md/editormd.min.js";
$(function() {
  var editor = editormd("test-editor", {
    // width  : "100%",
    // height : "100%",
    // path: "editor.md/editormd.min.js"
  });
});
export default {
  layout: "backstage-layout"
};
</script>
<style scoped lang="less">
</style>