<script lang="ts">
	import { GeoJSON, Map, TileLayer} from 'sveaflet';
	import COZIPS from '$lib/static/CDPHE_Open_Data_Colorado_ZIP_Code_Tabulation_Areas_(ZCTA)_2020.json'

</script>

<div class="map">
	<Map
		options={{
			center: [39.769237, -104.986703],
			zoom: 10.5			
		}}
	>
		<TileLayer url={'https://tile.openstreetmap.org/{z}/{x}/{y}.png'} />
		<GeoJSON json={COZIPS}/>
	</Map>
</div>

<style>
	.map {
		width:100%;
		height:55em;		
	}
</style>