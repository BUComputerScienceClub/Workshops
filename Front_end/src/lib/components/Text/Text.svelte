<script>
    import styles from './Text.module.css';

    export let message;
    export let sender;

</script>

<div class={styles["text"]}>
    <h4 class={styles["text-message"]}>{message}</h4>
    <div class={styles["text-sender"]}>{sender}</div>
</div>