<script>
$: injectedStyles = () => `* { background-color: red }`

$: injectedStyleScript = () => {
  return `<style>${injectedStyles()}</style>`;
};
</script>
    
{@html injectedStyleScript()}