<script lang="ts">
	import { Map, TileLayer, Marker, Popup } from 'sveaflet';	

</script>

<div class="map">
	<Map
		options={{
			center: [39.769237, -104.986703],
			zoom: 10.5			
		}}
	>
		<TileLayer url={'https://tile.openstreetmap.org/{z}/{x}/{y}.png'} />
	</Map>
</div>

<style>
	.map {
		width:100%;
		height:55em;		
	}
</style>