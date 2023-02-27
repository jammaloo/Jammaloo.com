<script>

</script>

<div class="outer-frame">
    <div class="inner-frame">
        <div class="inner-inner-frame">
            <div class="picture">
                <slot />
            </div>
        </div>
    </div>
</div>

<style>
.outer-frame {
    border: 1em solid var(--dark);
    background: var(--dark);
}

.inner-frame {
    border: 0.25em dashed var(--light);
    background: var(--bg);
}

.inner-inner-frame {
    border: 1em solid var(--dark);
    background: var(--light);
}

.picture {
    border: 2em solid var(--light);
    background: var(--bg);
    display: flex;
    justify-content: center;
    align-items: center;
}
</style>
