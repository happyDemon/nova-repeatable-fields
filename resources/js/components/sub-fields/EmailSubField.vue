<template>
    <div>
        <input
            :id="subField.name"
            :name="subField.name"
            type="email"
            class="w-full form-control form-input form-input-bordered"
            :value="value"
            :placeholder="subField.placeholder"
            @input="$emit('input', $event.target.value)"
        />
    </div>

</template>

<script>

    export default {

        props: [
            'subField',
            'value'
        ],

    }
</script>