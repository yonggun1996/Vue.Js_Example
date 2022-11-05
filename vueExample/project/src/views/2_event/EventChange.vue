<template>
  <div>
    <select name="" id="" @change="changeCity" v-model="selectedCity">
        <option value="">==도시선택==</option>
        <option :value="city.cityCode" :key="city.code" v-for="city in cityList">{{city.title}}</option>
    </select>
    <select name="" id="">
        <option :value="team.name" :key="team.name" v-for="team in selectedTeamList">{{team.name + " " + team.title}}</option>
    </select>
    <select name="" id="">
        <option :value="team.name" :key="team.name" v-for="team in selectedTeamList.filter(
            (team) => team.cityCode === this.selectedCity
        )">{{team.name + " " + team.title}}</option>
    </select>
  </div>
</template>

<script>
export default {
    data() {
        return {
            selectedCity: '',
            cityList: [
                {cityCode:'02', title:'서울'},
                {cityCode:'051', title:'부산'},
                {cityCode:'032', title:'인천'},
            ],
            teamName: [
                {cityCode:'02', name:'두산', title:'베어스'},
                {cityCode:'02', name:'LG', title:'트윈스'},
                {cityCode:'02', name:'키움', title:'히어로즈'},
                {cityCode:'051', name:'롯데', title:'자이언츠'},
                {cityCode:'032', name:'SSG', title:'랜더스'}
            ],
            selectedTeamList: []
        }
    },
    methods: {
        changeCity() {
            this.selectedTeamList = this.teamName.filter(
                team => team.cityCode === this.selectedCity
            )
        }
    }
}
</script>

<style>

</style>