<template>
    <div>
        <DashNav />
        <section id="pagecontent">
            <DashSide />
            <div class="main_crumb">
                <router-link to="/dashboard">Home</router-link>
                <span>/</span>
                <router-link to="/add-growth-devotional">Add Growth Devotional</router-link>
            </div>
            <div class="main_body">
                <div class="container-fluid">
                    <div class="row">
                        <div class="col-sm-12">
                            <div class="btnrows">
                                <router-link to='/growth-plans' class='btn btn-add'>
                                    <i class='fa fa-plus-circle'></i> Growth Plans
                                </router-link>
                                <router-link to='/growth-devotionals' class='btn btn-list'>
                                    <i class='fa fa-bars'></i> Growth Devotionals
                                </router-link>
                            </div>
                        </div>
                    </div>
                    <div class="row">
                        <div class="col-sm-12">
                            <div class="main_lord">
                                <router-link 
                                    to="/growth-devotionals" 
                                    class="btn pull-right btn-primary">LIST DEVOTIONALS
                                </router-link>
                                <h1>Add Growth Devotional</h1>
                                <AddGrowthDevForm />
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </section>
    </div>
</template>

<style scoped>

</style>

<script>
import DashNav from '../inc/DashNav'
import DashSide from '../inc/DashSide'
import AddGrowthDevForm from '../forms/AddGrowthDevForm'

export default {
	components: {
        DashNav,
        DashSide,
        AddGrowthDevForm
	}
}
</script>
