<script>
export let padding = true;

</script>

<div class="outer-frame">
    <div class="inner-frame">
        <div class="inner-inner-frame">
            <div class="picture" class:padding={padding}>
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
    border: 1.5em solid var(--light);
    background: var(--white);
    display: flex;
    justify-content: center;
    align-items: center;
}
.padding {
    padding: 1em;
}
</style>
