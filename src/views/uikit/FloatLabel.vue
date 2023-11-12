<script setup>
import { ref } from 'vue';

const calendarValue = ref(null);


const dropdownItems = ref([
    { name: 'Option 1', code: 'Option 1' },
    { name: 'Option 2', code: 'Option 2' },
    { name: 'Option 3', code: 'Option 3' }
]);

const dropdownItem = ref(null);
</script>

<template>
    <div class="grid">
        <div class="col-12 md:col-12">
            <div class="card p-fluid">
                <h5>Consumir API REST Empleado</h5>
                <div class="field">
                    <label for="nom">Nombre(S):</label>
                    <InputText id="nom" type="text" />
                </div>
                <div class="field">
                    <label for="salario">Salario:</label>
                    <InputText id="salario" type="text" />
                </div>
                <div class="field">
                    <label for="edad">Edad:</label>
                    <InputText id="edad" type="text" />
                </div>
                <div class="field">
                    <label for="idem">Id Emp:</label>
                    <InputText id="idem" type="text" />
                </div>
                <div class="col-12 md:col-6">
                    <Button label="Consultar datos" class="p-button-success mr-2 mb-2" icon="pi pi-search"/>
                </div>
            </div>
        </div>
    </div>
</template>
