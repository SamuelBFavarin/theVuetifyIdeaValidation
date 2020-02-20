<template>
  <v-item-group mandatory>
    <v-container fluid>
      <v-row>
        <v-col cols="12">
					
					<v-row :align="alignment" :justify="justify" style="height: 300px;">						
						<!-- CARDS -->

						<v-card class="mx-auto" width="200" height="200">
							<v-col class="menu_icon" cols="auto">
								<v-icon class="justify-center" x-large color="green darken-2" >contacts</v-icon>
								<p class="justify-center">Usuários</p>
							</v-col>
						</v-card>								

						<v-card class="mx-auto" width="200" height="200">
							<v-col class="menu_icon" cols="auto">
								<v-icon large color="purple darken-2">email</v-icon>
								<p class="justify-center">Access Control</p>
							</v-col>
						</v-card>	
						
	
						<v-card class="mx-auto" width="200" height="200">
							<v-col class="menu_icon" cols="auto">
								<v-icon large color="teal darken-2">gesture</v-icon>
								<p class="justify-center">Signature</p>
							</v-col>
						</v-card>	

	
						<v-card class="mx-auto" width="200" height="200">
							<v-col class="menu_icon" cols="auto">
								<v-icon large color="orange darken-2">send</v-icon>
								<p class="justify-center">Transfer</p>
							</v-col>
						</v-card>	
					</v-row>
        </v-col>
      </v-row>
    </v-container>
  </v-item-group>
</template>

<script>

export default {
  name: 'MenuMain',

  data: () => ({
    //
  }),
};
</script>

<style scoped>

	.menu_icon {
		text-align: center;
		margin-top: 45px;
	}

</style>