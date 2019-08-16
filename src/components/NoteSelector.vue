<template>
  <div class="note-selector">
    <p class="note-selector-title">First note...</p>
    <p class="note-selector-timestamp">Timestamp here...</p>
  </div>
</template>

<script>
export default {
  name: 'note-selector',
  props: ['note', 'selectedNoteId'],
  methods: {
    setSelectedNoteId: function(noteId) {
      this.$emit("selectNote", noteId)
    }
  }
}
</script>