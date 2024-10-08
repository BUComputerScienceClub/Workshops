<script>
    import styles from './Text.module.css';

    export let me;
    export let message;
    export let sender;
    export let time;

</script>

<div class={sender === me ? styles["text-owner"] : styles["text"]}>
    <div class={styles["text-sender"]}>{sender} :
        <small class={styles["text-time"]}>{time} </small>
    </div>
    <h4 class={styles["text-message"]}>{message}
    </h4>
</div>