<script>
  import { _ } from 'svelte-i18n'
</script>

<ol>
  <li>{$_('introduction.location_once')}</li>
  <li>{$_('introduction.data_device')}</li>
</ol>

<style>
@media screen and (max-width: 550px) {

  ol {
  flex-direction: column;
  align-items: center;
  }
}

ol {
  list-style: none;
  counter-reset: my-awesome-counter;
  display: flex;
  margin: 0;
  padding: 0;
}
ol li {
  counter-increment: my-awesome-counter;
  display: flex;
  width: 50%;
  font-size: 1rem;
  margin-bottom: 0.5rem;
}
ol li::before {
  content: counter(my-awesome-counter);
  font-weight: bold;
  font-size: 3rem;
  margin-right: -0.5rem;
  line-height: 1;
  color: #67b6ff6c;
  /* color: #ff676781 */
}
</style>
