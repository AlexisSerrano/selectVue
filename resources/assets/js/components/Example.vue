<template>
<div class="container">
    <div class="row">
        <div class="col-md-8 col-md-offset-2">
            <div class="panel panel-default">
                <div class="panel-heading">Example Component</div>
                <div class="panel-body">
                    <select2 :options="options" v-model="selected">
                        <option disabled value="0">Select one</option>
                    </select2>
                </div>
            </div>
        </div>
    </div>
</div>
</template>

<script>

export default {
    mounted() {
        console.log('Component mounted.')
    },
    data: function(){
        return {
            selected: 2,
            options:[
                {id:1,text:'hello'},
                {id:2,text:'hello 2'},
            ]
        }
    }
}
</script>