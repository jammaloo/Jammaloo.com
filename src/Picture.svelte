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
    display: inline-block;
}

.inner-frame {
    border: 0.25em dashed var(--light);
    background: var(--bg);
    display: inline-block;
}

.inner-inner-frame {
    border: 1em solid var(--dark);
    background: var(--light);
    display: inline-block;
}

.picture {
    border: 2em solid var(--light);
    background: var(--bg);
    display: flex;
    justify-content: center;
    align-items: center;
}
</style>
