[ev_charging_stations_map.html](https://github.com/user-attachments/files/25686109/ev_charging_stations_map.html)
<!DOCTYPE html>
<html></html>
<head>
    
    <meta http-equiv="content-type" content="text/html; charset=UTF-8" />
    <script src="https://cdn.jsdelivr.net/npm/leaflet@1.9.3/dist/leaflet.js"></script>
    <script src="https://code.jquery.com/jquery-3.7.1.min.js"></script>
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.2.2/dist/js/bootstrap.bundle.min.js"></script>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/Leaflet.awesome-markers/2.0.2/leaflet.awesome-markers.js"></script>
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/leaflet@1.9.3/dist/leaflet.css"/>
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap@5.2.2/dist/css/bootstrap.min.css"/>
    <link rel="stylesheet" href="https://netdna.bootstrapcdn.com/bootstrap/3.0.0/css/bootstrap-glyphicons.css"/>
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/@fortawesome/fontawesome-free@6.2.0/css/all.min.css"/>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/Leaflet.awesome-markers/2.0.2/leaflet.awesome-markers.css"/>
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/gh/python-visualization/folium/folium/templates/leaflet.awesome.rotate.min.css"/>
    
            <meta name="viewport" content="width=device-width,
                initial-scale=1.0, maximum-scale=1.0, user-scalable=no" />
            <style>
                #map_c8ff09de98adc905a54fc2040c1d5971 {
                    position: relative;
                    width: 100.0%;
                    height: 100.0%;
                    left: 0.0%;
                    top: 0.0%;
                }
                .leaflet-container { font-size: 1rem; }
            </style>

            <style>html, body {
                width: 100%;
                height: 100%;
                margin: 0;
                padding: 0;
            }
            </style>

            <style>#map {
                position:absolute;
                top:0;
                bottom:0;
                right:0;
                left:0;
                }
            </style>

            <script>
                L_NO_TOUCH = false;
                L_DISABLE_3D = false;
            </script>

        
    <script src="https://cdn.jsdelivr.net/gh/python-visualization/folium@main/folium/templates/leaflet_heat.min.js"></script>
</head>
<body>
    
    
             <div style="position: fixed; 
                     top: 10px; left: 50px; width: 350px; height: auto; 
                     background-color: white; border:2px solid grey; z-index:9999; 
                     font-size:13px; font-weight: bold; border-radius: 5px; padding: 10px">
             🗺️ HANOI EV CHARGING STATION MAP
             <hr style="margin: 5px 0">
             <span style="color: green">● Green: Selected ✅</span><br>
             <span style="color: red">● Red: Not selected ❌</span><br>
             <span style="color: darkgreen">━ Coverage circle</span><br>
             <span style="color: orange">▲ Heatmap: Station density</span>
             </div>
             
    
            <div class="folium-map" id="map_c8ff09de98adc905a54fc2040c1d5971" ></div>
        
</body>
<script>
    
    
            var map_c8ff09de98adc905a54fc2040c1d5971 = L.map(
                "map_c8ff09de98adc905a54fc2040c1d5971",
                {
                    center: [21.0172713858685, 105.82011045592768],
                    crs: L.CRS.EPSG3857,
                    ...{
  "zoom": 11,
  "zoomControl": true,
  "preferCanvas": false,
}

                }
            );

            

        
    
            var tile_layer_d949b83fe6f517e896e0f6c4843cfe36 = L.tileLayer(
                "https://tile.openstreetmap.org/{z}/{x}/{y}.png",
                {
  "minZoom": 0,
  "maxZoom": 19,
  "maxNativeZoom": 19,
  "noWrap": false,
  "attribution": "\u0026copy; \u003ca href=\"https://www.openstreetmap.org/copyright\"\u003eOpenStreetMap\u003c/a\u003e contributors",
  "subdomains": "abc",
  "detectRetina": false,
  "tms": false,
  "opacity": 1,
}

            );
        
    
            tile_layer_d949b83fe6f517e896e0f6c4843cfe36.addTo(map_c8ff09de98adc905a54fc2040c1d5971);
        
    
            var marker_3f590acaa38af967496d4a7ce6812e2d = L.marker(
                [21.0375882767599, 105.836016798972],
                {
}
            ).addTo(map_c8ff09de98adc905a54fc2040c1d5971);
        
    
            var icon_dc18ad97906d87525feafb6f7338a80f = L.AwesomeMarkers.icon(
                {
  "markerColor": "red",
  "iconColor": "white",
  "icon": "times",
  "prefix": "fa",
  "extraClasses": "fa-rotate-0",
}
            );
        
    
        var popup_f2e3216249c72ae73e52b4d74b15f807 = L.popup({
  "maxWidth": 350,
});

        
            
                var html_11e9fea6007169736ec92967d0c64dbd = $(`<div id="html_11e9fea6007169736ec92967d0c64dbd" style="width: 100.0%; height: 100.0%;">         <b style='font-size:12px'>Quảng trường Ba Đình</b><br>         <hr style='margin:3px 0'>         <b>❌ NOT SELECTED</b><br>         ID: Site_01<br>         District: D_02<br>         <br>         <b>🏗️ Infrastructure:</b><br>         • Area: 80 m²<br>         • Grid Power: 500 kW<br>         • Base Load: 900 kW<br>         • Base Cost: 250,000,000 VND         </div>`)[0];
                popup_f2e3216249c72ae73e52b4d74b15f807.setContent(html_11e9fea6007169736ec92967d0c64dbd);
            
        

        marker_3f590acaa38af967496d4a7ce6812e2d.bindPopup(popup_f2e3216249c72ae73e52b4d74b15f807)
        ;

        
    
    
            marker_3f590acaa38af967496d4a7ce6812e2d.bindTooltip(
                `<div>
                     Quảng trường Ba Đình (❌ NOT SELECTED)
                 </div>`,
                {
  "sticky": true,
}
            );
        
    
                marker_3f590acaa38af967496d4a7ce6812e2d.setIcon(icon_dc18ad97906d87525feafb6f7338a80f);
            
    
            var marker_a4f037c05a25ab49df8b4d4f8a667c03 = L.marker(
                [21.0321415763038, 105.809331852041],
                {
}
            ).addTo(map_c8ff09de98adc905a54fc2040c1d5971);
        
    
            var icon_78b78dec73b94a4b97df30541615ddca = L.AwesomeMarkers.icon(
                {
  "markerColor": "red",
  "iconColor": "white",
  "icon": "times",
  "prefix": "fa",
  "extraClasses": "fa-rotate-0",
}
            );
        
    
        var popup_90368797e5ed9cbec07c68429778fd84 = L.popup({
  "maxWidth": 350,
});

        
            
                var html_5504a76a32285317ea6896617441b88b = $(`<div id="html_5504a76a32285317ea6896617441b88b" style="width: 100.0%; height: 100.0%;">         <b style='font-size:12px'>Bãi đỗ xe công viên Thủ Lệ</b><br>         <hr style='margin:3px 0'>         <b>❌ NOT SELECTED</b><br>         ID: Site_02<br>         District: D_02<br>         <br>         <b>🏗️ Infrastructure:</b><br>         • Area: 90 m²<br>         • Grid Power: 400 kW<br>         • Base Load: 700 kW<br>         • Base Cost: 200,000,000 VND         </div>`)[0];
                popup_90368797e5ed9cbec07c68429778fd84.setContent(html_5504a76a32285317ea6896617441b88b);
            
        

        marker_a4f037c05a25ab49df8b4d4f8a667c03.bindPopup(popup_90368797e5ed9cbec07c68429778fd84)
        ;

        
    
    
            marker_a4f037c05a25ab49df8b4d4f8a667c03.bindTooltip(
                `<div>
                     Bãi đỗ xe công viên Thủ Lệ (❌ NOT SELECTED)
                 </div>`,
                {
  "sticky": true,
}
            );
        
    
                marker_a4f037c05a25ab49df8b4d4f8a667c03.setIcon(icon_78b78dec73b94a4b97df30541615ddca);
            
    
            var marker_6b26c5a53a2f2faff66663655f121530 = L.marker(
                [21.0180245263029, 105.816901052041],
                {
}
            ).addTo(map_c8ff09de98adc905a54fc2040c1d5971);
        
    
            var icon_3b17e3016a68f53730cba3764dab00bd = L.AwesomeMarkers.icon(
                {
  "markerColor": "red",
  "iconColor": "white",
  "icon": "times",
  "prefix": "fa",
  "extraClasses": "fa-rotate-0",
}
            );
        
    
        var popup_df9b57dafa352212c7f8598c80db8a88 = L.popup({
  "maxWidth": 350,
});

        
            
                var html_96c06b8d2ca27155fd6b9a4512c461af = $(`<div id="html_96c06b8d2ca27155fd6b9a4512c461af" style="width: 100.0%; height: 100.0%;">         <b style='font-size:12px'>Bãi đỗ xe 81 Láng Hạ</b><br>         <hr style='margin:3px 0'>         <b>❌ NOT SELECTED</b><br>         ID: Site_03<br>         District: D_02<br>         <br>         <b>🏗️ Infrastructure:</b><br>         • Area: 70 m²<br>         • Grid Power: 400 kW<br>         • Base Load: 650 kW<br>         • Base Cost: 220,000,000 VND         </div>`)[0];
                popup_df9b57dafa352212c7f8598c80db8a88.setContent(html_96c06b8d2ca27155fd6b9a4512c461af);
            
        

        marker_6b26c5a53a2f2faff66663655f121530.bindPopup(popup_df9b57dafa352212c7f8598c80db8a88)
        ;

        
    
    
            marker_6b26c5a53a2f2faff66663655f121530.bindTooltip(
                `<div>
                     Bãi đỗ xe 81 Láng Hạ (❌ NOT SELECTED)
                 </div>`,
                {
  "sticky": true,
}
            );
        
    
                marker_6b26c5a53a2f2faff66663655f121530.setIcon(icon_3b17e3016a68f53730cba3764dab00bd);
            
    
            var marker_883bdb94a7a510089568ebdf0d4437ab = L.marker(
                [21.0238122587712, 105.812943825055],
                {
}
            ).addTo(map_c8ff09de98adc905a54fc2040c1d5971);
        
    
            var icon_006e6cc4d6e6d42f911102bb0ae41acc = L.AwesomeMarkers.icon(
                {
  "markerColor": "red",
  "iconColor": "white",
  "icon": "times",
  "prefix": "fa",
  "extraClasses": "fa-rotate-0",
}
            );
        
    
        var popup_c6cd139659aa01cf0c8d3906baf5b1ba = L.popup({
  "maxWidth": 350,
});

        
            
                var html_796231dafcc4a2d234719eba50f5352c = $(`<div id="html_796231dafcc4a2d234719eba50f5352c" style="width: 100.0%; height: 100.0%;">         <b style='font-size:12px'>D6 Thành Công</b><br>         <hr style='margin:3px 0'>         <b>❌ NOT SELECTED</b><br>         ID: Site_04<br>         District: D_02<br>         <br>         <b>🏗️ Infrastructure:</b><br>         • Area: 60 m²<br>         • Grid Power: 300 kW<br>         • Base Load: 500 kW<br>         • Base Cost: 180,000,000 VND         </div>`)[0];
                popup_c6cd139659aa01cf0c8d3906baf5b1ba.setContent(html_796231dafcc4a2d234719eba50f5352c);
            
        

        marker_883bdb94a7a510089568ebdf0d4437ab.bindPopup(popup_c6cd139659aa01cf0c8d3906baf5b1ba)
        ;

        
    
    
            marker_883bdb94a7a510089568ebdf0d4437ab.bindTooltip(
                `<div>
                     D6 Thành Công (❌ NOT SELECTED)
                 </div>`,
                {
  "sticky": true,
}
            );
        
    
                marker_883bdb94a7a510089568ebdf0d4437ab.setIcon(icon_006e6cc4d6e6d42f911102bb0ae41acc);
            
    
            var marker_0a5cd92c6a16602f820d194f95b967e7 = L.marker(
                [21.0475545153838, 105.83722099437],
                {
}
            ).addTo(map_c8ff09de98adc905a54fc2040c1d5971);
        
    
            var icon_972bebacfb988009634eca6257aaa943 = L.AwesomeMarkers.icon(
                {
  "markerColor": "red",
  "iconColor": "white",
  "icon": "times",
  "prefix": "fa",
  "extraClasses": "fa-rotate-0",
}
            );
        
    
        var popup_1106ebe3e8eedcfd1fc9ab523539391a = L.popup({
  "maxWidth": 350,
});

        
            
                var html_b873daa8370a2e1a24d77baa9078897d = $(`<div id="html_b873daa8370a2e1a24d77baa9078897d" style="width: 100.0%; height: 100.0%;">         <b style='font-size:12px'>Đường thanh niên</b><br>         <hr style='margin:3px 0'>         <b>❌ NOT SELECTED</b><br>         ID: Site_05<br>         District: D_02<br>         <br>         <b>🏗️ Infrastructure:</b><br>         • Area: 70 m²<br>         • Grid Power: 350 kW<br>         • Base Load: 600 kW<br>         • Base Cost: 200,000,000 VND         </div>`)[0];
                popup_1106ebe3e8eedcfd1fc9ab523539391a.setContent(html_b873daa8370a2e1a24d77baa9078897d);
            
        

        marker_0a5cd92c6a16602f820d194f95b967e7.bindPopup(popup_1106ebe3e8eedcfd1fc9ab523539391a)
        ;

        
    
    
            marker_0a5cd92c6a16602f820d194f95b967e7.bindTooltip(
                `<div>
                     Đường thanh niên (❌ NOT SELECTED)
                 </div>`,
                {
  "sticky": true,
}
            );
        
    
                marker_0a5cd92c6a16602f820d194f95b967e7.setIcon(icon_972bebacfb988009634eca6257aaa943);
            
    
            var marker_426697160fc0a77af0ff09c827faea74 = L.marker(
                [21.0314358642478, 105.814703707863],
                {
}
            ).addTo(map_c8ff09de98adc905a54fc2040c1d5971);
        
    
            var icon_d5cc3d9a67f425ce3cc7dc5e71bc19e8 = L.AwesomeMarkers.icon(
                {
  "markerColor": "red",
  "iconColor": "white",
  "icon": "times",
  "prefix": "fa",
  "extraClasses": "fa-rotate-0",
}
            );
        
    
        var popup_3cfe3aaa8bfcb9ab88b500c00c70097c = L.popup({
  "maxWidth": 350,
});

        
            
                var html_78fca66be3c18a4db64b78c9f2dfd1ae = $(`<div id="html_78fca66be3c18a4db64b78c9f2dfd1ae" style="width: 100.0%; height: 100.0%;">         <b style='font-size:12px'>Vincom Center Metropolis</b><br>         <hr style='margin:3px 0'>         <b>❌ NOT SELECTED</b><br>         ID: Site_06<br>         District: D_02<br>         <br>         <b>🏗️ Infrastructure:</b><br>         • Area: 100 m²<br>         • Grid Power: 500 kW<br>         • Base Load: 1000 kW<br>         • Base Cost: 300,000,000 VND         </div>`)[0];
                popup_3cfe3aaa8bfcb9ab88b500c00c70097c.setContent(html_78fca66be3c18a4db64b78c9f2dfd1ae);
            
        

        marker_426697160fc0a77af0ff09c827faea74.bindPopup(popup_3cfe3aaa8bfcb9ab88b500c00c70097c)
        ;

        
    
    
            marker_426697160fc0a77af0ff09c827faea74.bindTooltip(
                `<div>
                     Vincom Center Metropolis (❌ NOT SELECTED)
                 </div>`,
                {
  "sticky": true,
}
            );
        
    
                marker_426697160fc0a77af0ff09c827faea74.setIcon(icon_d5cc3d9a67f425ce3cc7dc5e71bc19e8);
            
    
            var marker_43922b55ef8ba27a0f31186a843d91f0 = L.marker(
                [21.0324360462316, 105.812491167384],
                {
}
            ).addTo(map_c8ff09de98adc905a54fc2040c1d5971);
        
    
            var icon_f5898716e913f98d632c6069656e1fc9 = L.AwesomeMarkers.icon(
                {
  "markerColor": "red",
  "iconColor": "white",
  "icon": "times",
  "prefix": "fa",
  "extraClasses": "fa-rotate-0",
}
            );
        
    
        var popup_4cbbe9c2bec22423ced828b001ed6d82 = L.popup({
  "maxWidth": 350,
});

        
            
                var html_203689695dbe71668af1c07d5733f897 = $(`<div id="html_203689695dbe71668af1c07d5733f897" style="width: 100.0%; height: 100.0%;">         <b style='font-size:12px'>LOTTE Mart</b><br>         <hr style='margin:3px 0'>         <b>❌ NOT SELECTED</b><br>         ID: Site_07<br>         District: D_02<br>         <br>         <b>🏗️ Infrastructure:</b><br>         • Area: 100 m²<br>         • Grid Power: 500 kW<br>         • Base Load: 1100 kW<br>         • Base Cost: 300,000,000 VND         </div>`)[0];
                popup_4cbbe9c2bec22423ced828b001ed6d82.setContent(html_203689695dbe71668af1c07d5733f897);
            
        

        marker_43922b55ef8ba27a0f31186a843d91f0.bindPopup(popup_4cbbe9c2bec22423ced828b001ed6d82)
        ;

        
    
    
            marker_43922b55ef8ba27a0f31186a843d91f0.bindTooltip(
                `<div>
                     LOTTE Mart (❌ NOT SELECTED)
                 </div>`,
                {
  "sticky": true,
}
            );
        
    
                marker_43922b55ef8ba27a0f31186a843d91f0.setIcon(icon_f5898716e913f98d632c6069656e1fc9);
            
    
            var marker_cd764ee12ad01bb53361441af6fddcc6 = L.marker(
                [21.0392996253807, 105.828983750191],
                {
}
            ).addTo(map_c8ff09de98adc905a54fc2040c1d5971);
        
    
            var icon_06292034c9a541eb0c78c8f29ed1b0ee = L.AwesomeMarkers.icon(
                {
  "markerColor": "red",
  "iconColor": "white",
  "icon": "times",
  "prefix": "fa",
  "extraClasses": "fa-rotate-0",
}
            );
        
    
        var popup_c2c9672c2bb2a2d71080c5775ffe94e6 = L.popup({
  "maxWidth": 350,
});

        
            
                var html_2c5db84198485a389786b1e5248ca376 = $(`<div id="html_2c5db84198485a389786b1e5248ca376" style="width: 100.0%; height: 100.0%;">         <b style='font-size:12px'>Bãi đỗ xe Ngọc Hà</b><br>         <hr style='margin:3px 0'>         <b>❌ NOT SELECTED</b><br>         ID: Site_08<br>         District: D_02<br>         <br>         <b>🏗️ Infrastructure:</b><br>         • Area: 65 m²<br>         • Grid Power: 350 kW<br>         • Base Load: 650 kW<br>         • Base Cost: 200,000,000 VND         </div>`)[0];
                popup_c2c9672c2bb2a2d71080c5775ffe94e6.setContent(html_2c5db84198485a389786b1e5248ca376);
            
        

        marker_cd764ee12ad01bb53361441af6fddcc6.bindPopup(popup_c2c9672c2bb2a2d71080c5775ffe94e6)
        ;

        
    
    
            marker_cd764ee12ad01bb53361441af6fddcc6.bindTooltip(
                `<div>
                     Bãi đỗ xe Ngọc Hà (❌ NOT SELECTED)
                 </div>`,
                {
  "sticky": true,
}
            );
        
    
                marker_cd764ee12ad01bb53361441af6fddcc6.setIcon(icon_06292034c9a541eb0c78c8f29ed1b0ee);
            
    
            var marker_07e2b95a9383be5b98fc67d2738f4c4c = L.marker(
                [21.0265830829458, 105.85906609437],
                {
}
            ).addTo(map_c8ff09de98adc905a54fc2040c1d5971);
        
    
            var icon_988a57e5383301672753ae8d5b15b2a6 = L.AwesomeMarkers.icon(
                {
  "markerColor": "red",
  "iconColor": "white",
  "icon": "times",
  "prefix": "fa",
  "extraClasses": "fa-rotate-0",
}
            );
        
    
        var popup_3144eaf3759c5f1dd78d47858a8be19b = L.popup({
  "maxWidth": 350,
});

        
            
                var html_71ba8095d4ea28429c2c476b9cec1a74 = $(`<div id="html_71ba8095d4ea28429c2c476b9cec1a74" style="width: 100.0%; height: 100.0%;">         <b style='font-size:12px'>Bac Co Parking</b><br>         <hr style='margin:3px 0'>         <b>❌ NOT SELECTED</b><br>         ID: Site_09<br>         District: D_01<br>         <br>         <b>🏗️ Infrastructure:</b><br>         • Area: 60 m²<br>         • Grid Power: 300 kW<br>         • Base Load: 600 kW<br>         • Base Cost: 220,000,000 VND         </div>`)[0];
                popup_3144eaf3759c5f1dd78d47858a8be19b.setContent(html_71ba8095d4ea28429c2c476b9cec1a74);
            
        

        marker_07e2b95a9383be5b98fc67d2738f4c4c.bindPopup(popup_3144eaf3759c5f1dd78d47858a8be19b)
        ;

        
    
    
            marker_07e2b95a9383be5b98fc67d2738f4c4c.bindTooltip(
                `<div>
                     Bac Co Parking (❌ NOT SELECTED)
                 </div>`,
                {
  "sticky": true,
}
            );
        
    
                marker_07e2b95a9383be5b98fc67d2738f4c4c.setIcon(icon_988a57e5383301672753ae8d5b15b2a6);
            
    
            var marker_d59f678ad823ae46a2d13dc213f724a1 = L.marker(
                [21.0261753137041, 105.847323967384],
                {
}
            ).addTo(map_c8ff09de98adc905a54fc2040c1d5971);
        
    
            var icon_f7ca778969f1c0a7f404222101b8deea = L.AwesomeMarkers.icon(
                {
  "markerColor": "red",
  "iconColor": "white",
  "icon": "times",
  "prefix": "fa",
  "extraClasses": "fa-rotate-0",
}
            );
        
    
        var popup_f1c5fe0e1ba323dae83ae8e1baa3fb18 = L.popup({
  "maxWidth": 350,
});

        
            
                var html_3bb7e438533ecdaffb11993e6ef3ddde = $(`<div id="html_3bb7e438533ecdaffb11993e6ef3ddde" style="width: 100.0%; height: 100.0%;">         <b style='font-size:12px'>Bãi gửi xe Mirai</b><br>         <hr style='margin:3px 0'>         <b>❌ NOT SELECTED</b><br>         ID: Site_10<br>         District: D_01<br>         <br>         <b>🏗️ Infrastructure:</b><br>         • Area: 70 m²<br>         • Grid Power: 400 kW<br>         • Base Load: 800 kW<br>         • Base Cost: 250,000,000 VND         </div>`)[0];
                popup_f1c5fe0e1ba323dae83ae8e1baa3fb18.setContent(html_3bb7e438533ecdaffb11993e6ef3ddde);
            
        

        marker_d59f678ad823ae46a2d13dc213f724a1.bindPopup(popup_f1c5fe0e1ba323dae83ae8e1baa3fb18)
        ;

        
    
    
            marker_d59f678ad823ae46a2d13dc213f724a1.bindTooltip(
                `<div>
                     Bãi gửi xe Mirai (❌ NOT SELECTED)
                 </div>`,
                {
  "sticky": true,
}
            );
        
    
                marker_d59f678ad823ae46a2d13dc213f724a1.setIcon(icon_f7ca778969f1c0a7f404222101b8deea);
            
    
            var marker_f9e95da173141cba6954fb925ab74b6c = L.marker(
                [21.0273403780546, 105.859642931692],
                {
}
            ).addTo(map_c8ff09de98adc905a54fc2040c1d5971);
        
    
            var icon_8c077bc2b623f9a4a62ec2436ab0a4e1 = L.AwesomeMarkers.icon(
                {
  "markerColor": "green",
  "iconColor": "white",
  "icon": "bolt",
  "prefix": "fa",
  "extraClasses": "fa-rotate-0",
}
            );
        
    
        var popup_9c7f9089ca2476db95d206dcd805a1fa = L.popup({
  "maxWidth": 350,
});

        
            
                var html_a7610ae5f825755f442889f55b1d9205 = $(`<div id="html_a7610ae5f825755f442889f55b1d9205" style="width: 100.0%; height: 100.0%;">         <b style='font-size:12px'>DCAR XANH</b><br>         <hr style='margin:3px 0'>         <b>✅ SELECTED</b><br>         ID: Site_11<br>         District: D_01<br>         <br>         <b>📊 Specifications:</b><br>         • Chargers: <b>6</b> ports<br>         • Power: <b>900</b> kW<br>         • Output: <b>1,390</b> kWh/day<br>         • Capital: <b>3,780,000,000</b> Million VND<br>         <br>         <b>🏗️ Infrastructure:</b><br>         • Area: 50 m²<br>         • Grid Power: 300 kW<br>         • Base Load: 500 kW         </div>`)[0];
                popup_9c7f9089ca2476db95d206dcd805a1fa.setContent(html_a7610ae5f825755f442889f55b1d9205);
            
        

        marker_f9e95da173141cba6954fb925ab74b6c.bindPopup(popup_9c7f9089ca2476db95d206dcd805a1fa)
        ;

        
    
    
            marker_f9e95da173141cba6954fb925ab74b6c.bindTooltip(
                `<div>
                     DCAR XANH (✅ SELECTED)
                 </div>`,
                {
  "sticky": true,
}
            );
        
    
                marker_f9e95da173141cba6954fb925ab74b6c.setIcon(icon_8c077bc2b623f9a4a62ec2436ab0a4e1);
            
    
            var marker_80e950de2e62359a11fdbcea3f560306 = L.marker(
                [21.0214173062508, 105.861597994369],
                {
}
            ).addTo(map_c8ff09de98adc905a54fc2040c1d5971);
        
    
            var icon_6d9f5ade1a4552837272496ce43556e8 = L.AwesomeMarkers.icon(
                {
  "markerColor": "green",
  "iconColor": "white",
  "icon": "bolt",
  "prefix": "fa",
  "extraClasses": "fa-rotate-0",
}
            );
        
    
        var popup_92d4848a8ebaeb9d634636f0e462a229 = L.popup({
  "maxWidth": 350,
});

        
            
                var html_54091d80e3ffbe84e985358f45a59cb5 = $(`<div id="html_54091d80e3ffbe84e985358f45a59cb5" style="width: 100.0%; height: 100.0%;">         <b style='font-size:12px'>Nhà xe Vấn Quyên</b><br>         <hr style='margin:3px 0'>         <b>✅ SELECTED</b><br>         ID: Site_12<br>         District: D_01<br>         <br>         <b>📊 Specifications:</b><br>         • Chargers: <b>7</b> ports<br>         • Power: <b>1050</b> kW<br>         • Output: <b>1,680</b> kWh/day<br>         • Capital: <b>4,380,000,000</b> Million VND<br>         <br>         <b>🏗️ Infrastructure:</b><br>         • Area: 50 m²<br>         • Grid Power: 300 kW<br>         • Base Load: 450 kW         </div>`)[0];
                popup_92d4848a8ebaeb9d634636f0e462a229.setContent(html_54091d80e3ffbe84e985358f45a59cb5);
            
        

        marker_80e950de2e62359a11fdbcea3f560306.bindPopup(popup_92d4848a8ebaeb9d634636f0e462a229)
        ;

        
    
    
            marker_80e950de2e62359a11fdbcea3f560306.bindTooltip(
                `<div>
                     Nhà xe Vấn Quyên (✅ SELECTED)
                 </div>`,
                {
  "sticky": true,
}
            );
        
    
                marker_80e950de2e62359a11fdbcea3f560306.setIcon(icon_6d9f5ade1a4552837272496ce43556e8);
            
    
            var marker_86b7bb78898a1126da69cad5fc36fbb9 = L.marker(
                [21.0249669990316, 105.853306052041],
                {
}
            ).addTo(map_c8ff09de98adc905a54fc2040c1d5971);
        
    
            var icon_1cdc0b3604a6a407159ba48327427460 = L.AwesomeMarkers.icon(
                {
  "markerColor": "red",
  "iconColor": "white",
  "icon": "times",
  "prefix": "fa",
  "extraClasses": "fa-rotate-0",
}
            );
        
    
        var popup_85f3983201fcebe291adfd9d0994bc8f = L.popup({
  "maxWidth": 350,
});

        
            
                var html_60e49dfcd65afb97907687fc6bf2e169 = $(`<div id="html_60e49dfcd65afb97907687fc6bf2e169" style="width: 100.0%; height: 100.0%;">         <b style='font-size:12px'>Trang Tien Plaza</b><br>         <hr style='margin:3px 0'>         <b>❌ NOT SELECTED</b><br>         ID: Site_13<br>         District: D_01<br>         <br>         <b>🏗️ Infrastructure:</b><br>         • Area: 90 m²<br>         • Grid Power: 500 kW<br>         • Base Load: 1000 kW<br>         • Base Cost: 280,000,000 VND         </div>`)[0];
                popup_85f3983201fcebe291adfd9d0994bc8f.setContent(html_60e49dfcd65afb97907687fc6bf2e169);
            
        

        marker_86b7bb78898a1126da69cad5fc36fbb9.bindPopup(popup_85f3983201fcebe291adfd9d0994bc8f)
        ;

        
    
    
            marker_86b7bb78898a1126da69cad5fc36fbb9.bindTooltip(
                `<div>
                     Trang Tien Plaza (❌ NOT SELECTED)
                 </div>`,
                {
  "sticky": true,
}
            );
        
    
                marker_86b7bb78898a1126da69cad5fc36fbb9.setIcon(icon_1cdc0b3604a6a407159ba48327427460);
            
    
            var marker_d9fcf67510ac995ee8feb7fd1cf0faac = L.marker(
                [21.031712291026, 105.846469079027],
                {
}
            ).addTo(map_c8ff09de98adc905a54fc2040c1d5971);
        
    
            var icon_5766ef07b6f32f445fa678050bd71b0b = L.AwesomeMarkers.icon(
                {
  "markerColor": "red",
  "iconColor": "white",
  "icon": "times",
  "prefix": "fa",
  "extraClasses": "fa-rotate-0",
}
            );
        
    
        var popup_9a9c2ca1991e4090ad62d811aa9aa225 = L.popup({
  "maxWidth": 350,
});

        
            
                var html_3cdf7c9f9216d0125019ba448025075a = $(`<div id="html_3cdf7c9f9216d0125019ba448025075a" style="width: 100.0%; height: 100.0%;">         <b style='font-size:12px'>Trung Tâm Thương Mại Hàng Da</b><br>         <hr style='margin:3px 0'>         <b>❌ NOT SELECTED</b><br>         ID: Site_14<br>         District: D_01<br>         <br>         <b>🏗️ Infrastructure:</b><br>         • Area: 100 m²<br>         • Grid Power: 500 kW<br>         • Base Load: 1100 kW<br>         • Base Cost: 300,000,000 VND         </div>`)[0];
                popup_9a9c2ca1991e4090ad62d811aa9aa225.setContent(html_3cdf7c9f9216d0125019ba448025075a);
            
        

        marker_d9fcf67510ac995ee8feb7fd1cf0faac.bindPopup(popup_9a9c2ca1991e4090ad62d811aa9aa225)
        ;

        
    
    
            marker_d9fcf67510ac995ee8feb7fd1cf0faac.bindTooltip(
                `<div>
                     Trung Tâm Thương Mại Hàng Da (❌ NOT SELECTED)
                 </div>`,
                {
  "sticky": true,
}
            );
        
    
                marker_d9fcf67510ac995ee8feb7fd1cf0faac.setIcon(icon_5766ef07b6f32f445fa678050bd71b0b);
            
    
            var marker_a3197058f827c89bb544c195b110d29d = L.marker(
                [21.0246041577598, 105.85154329437],
                {
}
            ).addTo(map_c8ff09de98adc905a54fc2040c1d5971);
        
    
            var icon_4a423552a90e44a2501136918e3a7477 = L.AwesomeMarkers.icon(
                {
  "markerColor": "red",
  "iconColor": "white",
  "icon": "times",
  "prefix": "fa",
  "extraClasses": "fa-rotate-0",
}
            );
        
    
        var popup_758958c6b7ec3073c7a07bb93c887fc6 = L.popup({
  "maxWidth": 350,
});

        
            
                var html_be9ea457820a48f138ccaa7bda6a8acc = $(`<div id="html_be9ea457820a48f138ccaa7bda6a8acc" style="width: 100.0%; height: 100.0%;">         <b style='font-size:12px'>Central Building</b><br>         <hr style='margin:3px 0'>         <b>❌ NOT SELECTED</b><br>         ID: Site_15<br>         District: D_01<br>         <br>         <b>🏗️ Infrastructure:</b><br>         • Area: 90 m²<br>         • Grid Power: 400 kW<br>         • Base Load: 900 kW<br>         • Base Cost: 260,000,000 VND         </div>`)[0];
                popup_758958c6b7ec3073c7a07bb93c887fc6.setContent(html_be9ea457820a48f138ccaa7bda6a8acc);
            
        

        marker_a3197058f827c89bb544c195b110d29d.bindPopup(popup_758958c6b7ec3073c7a07bb93c887fc6)
        ;

        
    
    
            marker_a3197058f827c89bb544c195b110d29d.bindTooltip(
                `<div>
                     Central Building (❌ NOT SELECTED)
                 </div>`,
                {
  "sticky": true,
}
            );
        
    
                marker_a3197058f827c89bb544c195b110d29d.setIcon(icon_4a423552a90e44a2501136918e3a7477);
            
    
            var marker_487022e61230dd5382ed4bd55ff7f856 = L.marker(
                [21.0320277496415, 105.85157569437],
                {
}
            ).addTo(map_c8ff09de98adc905a54fc2040c1d5971);
        
    
            var icon_92d62aa9771b073e215117119bc7e0e2 = L.AwesomeMarkers.icon(
                {
  "markerColor": "red",
  "iconColor": "white",
  "icon": "times",
  "prefix": "fa",
  "extraClasses": "fa-rotate-0",
}
            );
        
    
        var popup_f3bbee9e4c9b658f17cf12f67e36efec = L.popup({
  "maxWidth": 350,
});

        
            
                var html_1e23cc548020a56430b0a97501ad3f2e = $(`<div id="html_1e23cc548020a56430b0a97501ad3f2e" style="width: 100.0%; height: 100.0%;">         <b style='font-size:12px'>Quảng trường Đông Kinh Nghĩa Thục</b><br>         <hr style='margin:3px 0'>         <b>❌ NOT SELECTED</b><br>         ID: Site_16<br>         District: D_01<br>         <br>         <b>🏗️ Infrastructure:</b><br>         • Area: 50 m²<br>         • Grid Power: 300 kW<br>         • Base Load: 700 kW<br>         • Base Cost: 200,000,000 VND         </div>`)[0];
                popup_f3bbee9e4c9b658f17cf12f67e36efec.setContent(html_1e23cc548020a56430b0a97501ad3f2e);
            
        

        marker_487022e61230dd5382ed4bd55ff7f856.bindPopup(popup_f3bbee9e4c9b658f17cf12f67e36efec)
        ;

        
    
    
            marker_487022e61230dd5382ed4bd55ff7f856.bindTooltip(
                `<div>
                     Quảng trường Đông Kinh Nghĩa Thục (❌ NOT SELECTED)
                 </div>`,
                {
  "sticky": true,
}
            );
        
    
                marker_487022e61230dd5382ed4bd55ff7f856.setIcon(icon_92d62aa9771b073e215117119bc7e0e2);
            
    
            var marker_61e71553d595c8fc70c048a78aec7bf7 = L.marker(
                [21.010042615067, 105.823861501479],
                {
}
            ).addTo(map_c8ff09de98adc905a54fc2040c1d5971);
        
    
            var icon_15916f2a36ba01a2468b63988809ec79 = L.AwesomeMarkers.icon(
                {
  "markerColor": "red",
  "iconColor": "white",
  "icon": "times",
  "prefix": "fa",
  "extraClasses": "fa-rotate-0",
}
            );
        
    
        var popup_7532778be78222850313f3e7809cb288 = L.popup({
  "maxWidth": 350,
});

        
            
                var html_f85e20558e5eb19f8d9f3b12c07e4f01 = $(`<div id="html_f85e20558e5eb19f8d9f3b12c07e4f01" style="width: 100.0%; height: 100.0%;">         <b style='font-size:12px'>Viettower Building</b><br>         <hr style='margin:3px 0'>         <b>❌ NOT SELECTED</b><br>         ID: Site_17<br>         District: D_06<br>         <br>         <b>🏗️ Infrastructure:</b><br>         • Area: 90 m²<br>         • Grid Power: 500 kW<br>         • Base Load: 900 kW<br>         • Base Cost: 240,000,000 VND         </div>`)[0];
                popup_7532778be78222850313f3e7809cb288.setContent(html_f85e20558e5eb19f8d9f3b12c07e4f01);
            
        

        marker_61e71553d595c8fc70c048a78aec7bf7.bindPopup(popup_7532778be78222850313f3e7809cb288)
        ;

        
    
    
            marker_61e71553d595c8fc70c048a78aec7bf7.bindTooltip(
                `<div>
                     Viettower Building (❌ NOT SELECTED)
                 </div>`,
                {
  "sticky": true,
}
            );
        
    
                marker_61e71553d595c8fc70c048a78aec7bf7.setIcon(icon_15916f2a36ba01a2468b63988809ec79);
            
    
            var marker_cc366cc5c0dbc720e56ba26201d24a70 = L.marker(
                [21.0190785404453, 105.824301509712],
                {
}
            ).addTo(map_c8ff09de98adc905a54fc2040c1d5971);
        
    
            var icon_11d1d47a1d40bdfe47983f206d17dcfa = L.AwesomeMarkers.icon(
                {
  "markerColor": "green",
  "iconColor": "white",
  "icon": "bolt",
  "prefix": "fa",
  "extraClasses": "fa-rotate-0",
}
            );
        
    
        var popup_d10305886d4b263d551834f885a6ed37 = L.popup({
  "maxWidth": 350,
});

        
            
                var html_e1e22d08c8726267b0f696eba1f489a2 = $(`<div id="html_e1e22d08c8726267b0f696eba1f489a2" style="width: 100.0%; height: 100.0%;">         <b style='font-size:12px'>Bãi gửi xe ở phố Hoàng Cầu</b><br>         <hr style='margin:3px 0'>         <b>✅ SELECTED</b><br>         ID: Site_18<br>         District: D_06<br>         <br>         <b>📊 Specifications:</b><br>         • Chargers: <b>8</b> ports<br>         • Power: <b>1200</b> kW<br>         • Output: <b>1,853</b> kWh/day<br>         • Capital: <b>5,000,000,000</b> Million VND<br>         <br>         <b>🏗️ Infrastructure:</b><br>         • Area: 75 m²<br>         • Grid Power: 400 kW<br>         • Base Load: 700 kW         </div>`)[0];
                popup_d10305886d4b263d551834f885a6ed37.setContent(html_e1e22d08c8726267b0f696eba1f489a2);
            
        

        marker_cc366cc5c0dbc720e56ba26201d24a70.bindPopup(popup_d10305886d4b263d551834f885a6ed37)
        ;

        
    
    
            marker_cc366cc5c0dbc720e56ba26201d24a70.bindTooltip(
                `<div>
                     Bãi gửi xe ở phố Hoàng Cầu (✅ SELECTED)
                 </div>`,
                {
  "sticky": true,
}
            );
        
    
                marker_cc366cc5c0dbc720e56ba26201d24a70.setIcon(icon_11d1d47a1d40bdfe47983f206d17dcfa);
            
    
            var marker_0606b88ee6ce5ceadfd5a41dcf1a23e9 = L.marker(
                [21.0020087704945, 105.823001023204],
                {
}
            ).addTo(map_c8ff09de98adc905a54fc2040c1d5971);
        
    
            var icon_cd0ee7bf0fd5ffc72c5b72fd9788a9ee = L.AwesomeMarkers.icon(
                {
  "markerColor": "green",
  "iconColor": "white",
  "icon": "bolt",
  "prefix": "fa",
  "extraClasses": "fa-rotate-0",
}
            );
        
    
        var popup_798bfae719aa9c4c15e925fd073814a9 = L.popup({
  "maxWidth": 350,
});

        
            
                var html_ef62c70a513f891a8a8d5fbe114d06d0 = $(`<div id="html_ef62c70a513f891a8a8d5fbe114d06d0" style="width: 100.0%; height: 100.0%;">         <b style='font-size:12px'>Bãi đỗ xe Trường Chinh</b><br>         <hr style='margin:3px 0'>         <b>✅ SELECTED</b><br>         ID: Site_19<br>         District: D_06<br>         <br>         <b>📊 Specifications:</b><br>         • Chargers: <b>8</b> ports<br>         • Power: <b>1200</b> kW<br>         • Output: <b>1,775</b> kWh/day<br>         • Capital: <b>4,980,000,000</b> Million VND<br>         <br>         <b>🏗️ Infrastructure:</b><br>         • Area: 70 m²<br>         • Grid Power: 350 kW<br>         • Base Load: 600 kW         </div>`)[0];
                popup_798bfae719aa9c4c15e925fd073814a9.setContent(html_ef62c70a513f891a8a8d5fbe114d06d0);
            
        

        marker_0606b88ee6ce5ceadfd5a41dcf1a23e9.bindPopup(popup_798bfae719aa9c4c15e925fd073814a9)
        ;

        
    
    
            marker_0606b88ee6ce5ceadfd5a41dcf1a23e9.bindTooltip(
                `<div>
                     Bãi đỗ xe Trường Chinh (✅ SELECTED)
                 </div>`,
                {
  "sticky": true,
}
            );
        
    
                marker_0606b88ee6ce5ceadfd5a41dcf1a23e9.setIcon(icon_cd0ee7bf0fd5ffc72c5b72fd9788a9ee);
            
    
            var marker_3a705c43f4dbae8f6189c9f6bd32c09e = L.marker(
                [21.0102051205881, 105.838166790669],
                {
}
            ).addTo(map_c8ff09de98adc905a54fc2040c1d5971);
        
    
            var icon_a626de325cd6302ef1bb1b1b9aa659ab = L.AwesomeMarkers.icon(
                {
  "markerColor": "green",
  "iconColor": "white",
  "icon": "bolt",
  "prefix": "fa",
  "extraClasses": "fa-rotate-0",
}
            );
        
    
        var popup_29c3c0e92d1accb430957128f0438272 = L.popup({
  "maxWidth": 350,
});

        
            
                var html_af49ab762498ae63af0e3e803fb1e6a4 = $(`<div id="html_af49ab762498ae63af0e3e803fb1e6a4" style="width: 100.0%; height: 100.0%;">         <b style='font-size:12px'>Bãi giữ xe đình Kim Liên</b><br>         <hr style='margin:3px 0'>         <b>✅ SELECTED</b><br>         ID: Site_20<br>         District: D_06<br>         <br>         <b>📊 Specifications:</b><br>         • Chargers: <b>8</b> ports<br>         • Power: <b>1200</b> kW<br>         • Output: <b>1,590</b> kWh/day<br>         • Capital: <b>4,980,000,000</b> Million VND<br>         <br>         <b>🏗️ Infrastructure:</b><br>         • Area: 60 m²<br>         • Grid Power: 300 kW<br>         • Base Load: 500 kW         </div>`)[0];
                popup_29c3c0e92d1accb430957128f0438272.setContent(html_af49ab762498ae63af0e3e803fb1e6a4);
            
        

        marker_3a705c43f4dbae8f6189c9f6bd32c09e.bindPopup(popup_29c3c0e92d1accb430957128f0438272)
        ;

        
    
    
            marker_3a705c43f4dbae8f6189c9f6bd32c09e.bindTooltip(
                `<div>
                     Bãi giữ xe đình Kim Liên (✅ SELECTED)
                 </div>`,
                {
  "sticky": true,
}
            );
        
    
                marker_3a705c43f4dbae8f6189c9f6bd32c09e.setIcon(icon_a626de325cd6302ef1bb1b1b9aa659ab);
            
    
            var marker_8dfadf481ecd767e16dd04703e28ec5e = L.marker(
                [21.0126971036958, 105.823982780876],
                {
}
            ).addTo(map_c8ff09de98adc905a54fc2040c1d5971);
        
    
            var icon_480fbe548c59fd152d5d085fc12ac801 = L.AwesomeMarkers.icon(
                {
  "markerColor": "green",
  "iconColor": "white",
  "icon": "bolt",
  "prefix": "fa",
  "extraClasses": "fa-rotate-0",
}
            );
        
    
        var popup_7da14a0bd9d20214ea04d00e4635eab7 = L.popup({
  "maxWidth": 350,
});

        
            
                var html_5ff8eee3cc09121650e422e6d98d2e61 = $(`<div id="html_5ff8eee3cc09121650e422e6d98d2e61" style="width: 100.0%; height: 100.0%;">         <b style='font-size:12px'>Công viên Đống Đa</b><br>         <hr style='margin:3px 0'>         <b>✅ SELECTED</b><br>         ID: Site_21<br>         District: D_06<br>         <br>         <b>📊 Specifications:</b><br>         • Chargers: <b>8</b> ports<br>         • Power: <b>1200</b> kW<br>         • Output: <b>1,471</b> kWh/day<br>         • Capital: <b>5,020,000,000</b> Million VND<br>         <br>         <b>🏗️ Infrastructure:</b><br>         • Area: 85 m²<br>         • Grid Power: 400 kW<br>         • Base Load: 800 kW         </div>`)[0];
                popup_7da14a0bd9d20214ea04d00e4635eab7.setContent(html_5ff8eee3cc09121650e422e6d98d2e61);
            
        

        marker_8dfadf481ecd767e16dd04703e28ec5e.bindPopup(popup_7da14a0bd9d20214ea04d00e4635eab7)
        ;

        
    
    
            marker_8dfadf481ecd767e16dd04703e28ec5e.bindTooltip(
                `<div>
                     Công viên Đống Đa (✅ SELECTED)
                 </div>`,
                {
  "sticky": true,
}
            );
        
    
                marker_8dfadf481ecd767e16dd04703e28ec5e.setIcon(icon_480fbe548c59fd152d5d085fc12ac801);
            
    
            var marker_3455a3d00352255e1eb471ba0d382ede = L.marker(
                [21.0081011573386, 105.82771805204],
                {
}
            ).addTo(map_c8ff09de98adc905a54fc2040c1d5971);
        
    
            var icon_06c5e247461c3ea62578f6373744df8c = L.AwesomeMarkers.icon(
                {
  "markerColor": "green",
  "iconColor": "white",
  "icon": "bolt",
  "prefix": "fa",
  "extraClasses": "fa-rotate-0",
}
            );
        
    
        var popup_9a1e0f7f41d3090a568595d6c3181425 = L.popup({
  "maxWidth": 350,
});

        
            
                var html_d24a31a30f4d68e15b5be93c934e5853 = $(`<div id="html_d24a31a30f4d68e15b5be93c934e5853" style="width: 100.0%; height: 100.0%;">         <b style='font-size:12px'>P. Chùa Bộc</b><br>         <hr style='margin:3px 0'>         <b>✅ SELECTED</b><br>         ID: Site_22<br>         District: D_06<br>         <br>         <b>📊 Specifications:</b><br>         • Chargers: <b>7</b> ports<br>         • Power: <b>1050</b> kW<br>         • Output: <b>1,232</b> kWh/day<br>         • Capital: <b>4,440,000,000</b> Million VND<br>         <br>         <b>🏗️ Infrastructure:</b><br>         • Area: 70 m²<br>         • Grid Power: 400 kW<br>         • Base Load: 850 kW         </div>`)[0];
                popup_9a1e0f7f41d3090a568595d6c3181425.setContent(html_d24a31a30f4d68e15b5be93c934e5853);
            
        

        marker_3455a3d00352255e1eb471ba0d382ede.bindPopup(popup_9a1e0f7f41d3090a568595d6c3181425)
        ;

        
    
    
            marker_3455a3d00352255e1eb471ba0d382ede.bindTooltip(
                `<div>
                     P. Chùa Bộc (✅ SELECTED)
                 </div>`,
                {
  "sticky": true,
}
            );
        
    
                marker_3455a3d00352255e1eb471ba0d382ede.setIcon(icon_06c5e247461c3ea62578f6373744df8c);
            
    
            var marker_2355a695a3d88d026b841bd22ea0a44e = L.marker(
                [21.0037721483514, 105.830583789792],
                {
}
            ).addTo(map_c8ff09de98adc905a54fc2040c1d5971);
        
    
            var icon_ab833ad763a138f5ee8d96575ea59b46 = L.AwesomeMarkers.icon(
                {
  "markerColor": "green",
  "iconColor": "white",
  "icon": "bolt",
  "prefix": "fa",
  "extraClasses": "fa-rotate-0",
}
            );
        
    
        var popup_1e3a4e350eae38dd8cd9ed44a13b9552 = L.popup({
  "maxWidth": 350,
});

        
            
                var html_f8181a61001a211e91e3e40a6a439568 = $(`<div id="html_f8181a61001a211e91e3e40a6a439568" style="width: 100.0%; height: 100.0%;">         <b style='font-size:12px'>Đại học Y Hà Nội</b><br>         <hr style='margin:3px 0'>         <b>✅ SELECTED</b><br>         ID: Site_23<br>         District: D_06<br>         <br>         <b>📊 Specifications:</b><br>         • Chargers: <b>10</b> ports<br>         • Power: <b>1500</b> kW<br>         • Output: <b>1,925</b> kWh/day<br>         • Capital: <b>6,220,000,000</b> Million VND<br>         <br>         <b>🏗️ Infrastructure:</b><br>         • Area: 90 m²<br>         • Grid Power: 500 kW<br>         • Base Load: 1000 kW         </div>`)[0];
                popup_1e3a4e350eae38dd8cd9ed44a13b9552.setContent(html_f8181a61001a211e91e3e40a6a439568);
            
        

        marker_2355a695a3d88d026b841bd22ea0a44e.bindPopup(popup_1e3a4e350eae38dd8cd9ed44a13b9552)
        ;

        
    
    
            marker_2355a695a3d88d026b841bd22ea0a44e.bindTooltip(
                `<div>
                     Đại học Y Hà Nội (✅ SELECTED)
                 </div>`,
                {
  "sticky": true,
}
            );
        
    
                marker_2355a695a3d88d026b841bd22ea0a44e.setIcon(icon_ab833ad763a138f5ee8d96575ea59b46);
            
    
            var marker_a3f49352460b89f4fdc394074f42e2e7 = L.marker(
                [21.0196704043724, 105.827735107862],
                {
}
            ).addTo(map_c8ff09de98adc905a54fc2040c1d5971);
        
    
            var icon_12e9936a531e94fd5e9d3cee5b4dec1c = L.AwesomeMarkers.icon(
                {
  "markerColor": "red",
  "iconColor": "white",
  "icon": "times",
  "prefix": "fa",
  "extraClasses": "fa-rotate-0",
}
            );
        
    
        var popup_46de289537c8c495a6c78d3d813b5a1c = L.popup({
  "maxWidth": 350,
});

        
            
                var html_e64e025768578160ba362507edc0ad59 = $(`<div id="html_e64e025768578160ba362507edc0ad59" style="width: 100.0%; height: 100.0%;">         <b style='font-size:12px'>P. Ô Chợ Dừa</b><br>         <hr style='margin:3px 0'>         <b>❌ NOT SELECTED</b><br>         ID: Site_24<br>         District: D_06<br>         <br>         <b>🏗️ Infrastructure:</b><br>         • Area: 75 m²<br>         • Grid Power: 400 kW<br>         • Base Load: 750 kW<br>         • Base Cost: 200,000,000 VND         </div>`)[0];
                popup_46de289537c8c495a6c78d3d813b5a1c.setContent(html_e64e025768578160ba362507edc0ad59);
            
        

        marker_a3f49352460b89f4fdc394074f42e2e7.bindPopup(popup_46de289537c8c495a6c78d3d813b5a1c)
        ;

        
    
    
            marker_a3f49352460b89f4fdc394074f42e2e7.bindTooltip(
                `<div>
                     P. Ô Chợ Dừa (❌ NOT SELECTED)
                 </div>`,
                {
  "sticky": true,
}
            );
        
    
                marker_a3f49352460b89f4fdc394074f42e2e7.setIcon(icon_12e9936a531e94fd5e9d3cee5b4dec1c);
            
    
            var marker_523ef938ffb23df9c11e46286bdc2e4b = L.marker(
                [21.0111497989239, 105.849558236698],
                {
}
            ).addTo(map_c8ff09de98adc905a54fc2040c1d5971);
        
    
            var icon_cd9d427f314db9f8c6c08dd476d0340d = L.AwesomeMarkers.icon(
                {
  "markerColor": "red",
  "iconColor": "white",
  "icon": "times",
  "prefix": "fa",
  "extraClasses": "fa-rotate-0",
}
            );
        
    
        var popup_924724661ad86474461d2e33f84fa73d = L.popup({
  "maxWidth": 350,
});

        
            
                var html_9e3f82b5aeb0c904463f13073b1ba12c = $(`<div id="html_9e3f82b5aeb0c904463f13073b1ba12c" style="width: 100.0%; height: 100.0%;">         <b style='font-size:12px'>Vincom Center Bà Triệu</b><br>         <hr style='margin:3px 0'>         <b>❌ NOT SELECTED</b><br>         ID: Site_25<br>         District: D_07<br>         <br>         <b>🏗️ Infrastructure:</b><br>         • Area: 100 m²<br>         • Grid Power: 500 kW<br>         • Base Load: 1100 kW<br>         • Base Cost: 300,000,000 VND         </div>`)[0];
                popup_924724661ad86474461d2e33f84fa73d.setContent(html_9e3f82b5aeb0c904463f13073b1ba12c);
            
        

        marker_523ef938ffb23df9c11e46286bdc2e4b.bindPopup(popup_924724661ad86474461d2e33f84fa73d)
        ;

        
    
    
            marker_523ef938ffb23df9c11e46286bdc2e4b.bindTooltip(
                `<div>
                     Vincom Center Bà Triệu (❌ NOT SELECTED)
                 </div>`,
                {
  "sticky": true,
}
            );
        
    
                marker_523ef938ffb23df9c11e46286bdc2e4b.setIcon(icon_cd9d427f314db9f8c6c08dd476d0340d);
            
    
            var marker_885943c0ea96f4a7f6965abe070c72d6 = L.marker(
                [20.9934769307658, 105.86855805204],
                {
}
            ).addTo(map_c8ff09de98adc905a54fc2040c1d5971);
        
    
            var icon_c257715adb55c61141bcd5f695f262dc = L.AwesomeMarkers.icon(
                {
  "markerColor": "green",
  "iconColor": "white",
  "icon": "bolt",
  "prefix": "fa",
  "extraClasses": "fa-rotate-0",
}
            );
        
    
        var popup_0e5424ee5eccbcb4e8699238c89eb9b3 = L.popup({
  "maxWidth": 350,
});

        
            
                var html_015d36b2c1d223eb46b7fda43168f1bc = $(`<div id="html_015d36b2c1d223eb46b7fda43168f1bc" style="width: 100.0%; height: 100.0%;">         <b style='font-size:12px'>Times City T11</b><br>         <hr style='margin:3px 0'>         <b>✅ SELECTED</b><br>         ID: Site_26<br>         District: D_07<br>         <br>         <b>📊 Specifications:</b><br>         • Chargers: <b>9</b> ports<br>         • Power: <b>1350</b> kW<br>         • Output: <b>5,439</b> kWh/day<br>         • Capital: <b>5,750,000,000</b> Million VND<br>         <br>         <b>🏗️ Infrastructure:</b><br>         • Area: 100 m²<br>         • Grid Power: 1000 kW<br>         • Base Load: 1200 kW         </div>`)[0];
                popup_0e5424ee5eccbcb4e8699238c89eb9b3.setContent(html_015d36b2c1d223eb46b7fda43168f1bc);
            
        

        marker_885943c0ea96f4a7f6965abe070c72d6.bindPopup(popup_0e5424ee5eccbcb4e8699238c89eb9b3)
        ;

        
    
    
            marker_885943c0ea96f4a7f6965abe070c72d6.bindTooltip(
                `<div>
                     Times City T11 (✅ SELECTED)
                 </div>`,
                {
  "sticky": true,
}
            );
        
    
                marker_885943c0ea96f4a7f6965abe070c72d6.setIcon(icon_c257715adb55c61141bcd5f695f262dc);
            
    
            var marker_270e0c6e8a4ea4c23a3579004f5423e5 = L.marker(
                [21.0173985669612, 105.845726767384],
                {
}
            ).addTo(map_c8ff09de98adc905a54fc2040c1d5971);
        
    
            var icon_1ea70883537a503a3dd5ec0b66d1aec3 = L.AwesomeMarkers.icon(
                {
  "markerColor": "red",
  "iconColor": "white",
  "icon": "times",
  "prefix": "fa",
  "extraClasses": "fa-rotate-0",
}
            );
        
    
        var popup_93419d2295bdd8b9b3c55479410135ca = L.popup({
  "maxWidth": 350,
});

        
            
                var html_585194b21120e4f1b26367b5774e630e = $(`<div id="html_585194b21120e4f1b26367b5774e630e" style="width: 100.0%; height: 100.0%;">         <b style='font-size:12px'>Công viên Thống Nhất</b><br>         <hr style='margin:3px 0'>         <b>❌ NOT SELECTED</b><br>         ID: Site_27<br>         District: D_07<br>         <br>         <b>🏗️ Infrastructure:</b><br>         • Area: 95 m²<br>         • Grid Power: 500 kW<br>         • Base Load: 900 kW<br>         • Base Cost: 250,000,000 VND         </div>`)[0];
                popup_93419d2295bdd8b9b3c55479410135ca.setContent(html_585194b21120e4f1b26367b5774e630e);
            
        

        marker_270e0c6e8a4ea4c23a3579004f5423e5.bindPopup(popup_93419d2295bdd8b9b3c55479410135ca)
        ;

        
    
    
            marker_270e0c6e8a4ea4c23a3579004f5423e5.bindTooltip(
                `<div>
                     Công viên Thống Nhất (❌ NOT SELECTED)
                 </div>`,
                {
  "sticky": true,
}
            );
        
    
                marker_270e0c6e8a4ea4c23a3579004f5423e5.setIcon(icon_1ea70883537a503a3dd5ec0b66d1aec3);
            
    
            var marker_948462a8c8d27a8bead3da64952daa6d = L.marker(
                [21.0020934059866, 105.840450180876],
                {
}
            ).addTo(map_c8ff09de98adc905a54fc2040c1d5971);
        
    
            var icon_8d24760a5a7981e155f8e4a7eb5c47ff = L.AwesomeMarkers.icon(
                {
  "markerColor": "red",
  "iconColor": "white",
  "icon": "times",
  "prefix": "fa",
  "extraClasses": "fa-rotate-0",
}
            );
        
    
        var popup_52bf5e9458766ac887ac0432c4fd7eef = L.popup({
  "maxWidth": 350,
});

        
            
                var html_157d8f088d0b76fedbab91e34ebdb5d3 = $(`<div id="html_157d8f088d0b76fedbab91e34ebdb5d3" style="width: 100.0%; height: 100.0%;">         <b style='font-size:12px'>Bãi xe ô tô P. Võ Thị Sáu</b><br>         <hr style='margin:3px 0'>         <b>❌ NOT SELECTED</b><br>         ID: Site_28<br>         District: D_07<br>         <br>         <b>🏗️ Infrastructure:</b><br>         • Area: 70 m²<br>         • Grid Power: 400 kW<br>         • Base Load: 700 kW<br>         • Base Cost: 220,000,000 VND         </div>`)[0];
                popup_52bf5e9458766ac887ac0432c4fd7eef.setContent(html_157d8f088d0b76fedbab91e34ebdb5d3);
            
        

        marker_948462a8c8d27a8bead3da64952daa6d.bindPopup(popup_52bf5e9458766ac887ac0432c4fd7eef)
        ;

        
    
    
            marker_948462a8c8d27a8bead3da64952daa6d.bindTooltip(
                `<div>
                     Bãi xe ô tô P. Võ Thị Sáu (❌ NOT SELECTED)
                 </div>`,
                {
  "sticky": true,
}
            );
        
    
                marker_948462a8c8d27a8bead3da64952daa6d.setIcon(icon_8d24760a5a7981e155f8e4a7eb5c47ff);
            
    
            var marker_dfeec41f6747008be4aaf1586357d33c = L.marker(
                [20.9998768080708, 105.869868065533],
                {
}
            ).addTo(map_c8ff09de98adc905a54fc2040c1d5971);
        
    
            var icon_5b8961a4f133b510b11981cf7fb3641f = L.AwesomeMarkers.icon(
                {
  "markerColor": "green",
  "iconColor": "white",
  "icon": "bolt",
  "prefix": "fa",
  "extraClasses": "fa-rotate-0",
}
            );
        
    
        var popup_fe9ed758d821244105d32308d5662853 = L.popup({
  "maxWidth": 350,
});

        
            
                var html_a3092fbdf26f0de72069540aa0f85986 = $(`<div id="html_a3092fbdf26f0de72069540aa0f85986" style="width: 100.0%; height: 100.0%;">         <b style='font-size:12px'>Hòa Bình Green City</b><br>         <hr style='margin:3px 0'>         <b>✅ SELECTED</b><br>         ID: Site_29<br>         District: D_07<br>         <br>         <b>📊 Specifications:</b><br>         • Chargers: <b>8</b> ports<br>         • Power: <b>1200</b> kW<br>         • Output: <b>4,080</b> kWh/day<br>         • Capital: <b>5,100,000,000</b> Million VND<br>         <br>         <b>🏗️ Infrastructure:</b><br>         • Area: 90 m²<br>         • Grid Power: 800 kW<br>         • Base Load: 1000 kW         </div>`)[0];
                popup_fe9ed758d821244105d32308d5662853.setContent(html_a3092fbdf26f0de72069540aa0f85986);
            
        

        marker_dfeec41f6747008be4aaf1586357d33c.bindPopup(popup_fe9ed758d821244105d32308d5662853)
        ;

        
    
    
            marker_dfeec41f6747008be4aaf1586357d33c.bindTooltip(
                `<div>
                     Hòa Bình Green City (✅ SELECTED)
                 </div>`,
                {
  "sticky": true,
}
            );
        
    
                marker_dfeec41f6747008be4aaf1586357d33c.setIcon(icon_5b8961a4f133b510b11981cf7fb3641f);
            
    
            var marker_b49f189ced40063eb198ed35de03d024 = L.marker(
                [21.0037361684065, 105.859374994369],
                {
}
            ).addTo(map_c8ff09de98adc905a54fc2040c1d5971);
        
    
            var icon_ac0d2c327770a002b45bb22b2692df1f = L.AwesomeMarkers.icon(
                {
  "markerColor": "red",
  "iconColor": "white",
  "icon": "times",
  "prefix": "fa",
  "extraClasses": "fa-rotate-0",
}
            );
        
    
        var popup_f4359f32f4d7bf285111773483d294c5 = L.popup({
  "maxWidth": 350,
});

        
            
                var html_fa9f070763d323db75b648e88339407a = $(`<div id="html_fa9f070763d323db75b648e88339407a" style="width: 100.0%; height: 100.0%;">         <b style='font-size:12px'>Bệnh viện Thanh Nhàn</b><br>         <hr style='margin:3px 0'>         <b>❌ NOT SELECTED</b><br>         ID: Site_30<br>         District: D_07<br>         <br>         <b>🏗️ Infrastructure:</b><br>         • Area: 70 m²<br>         • Grid Power: 400 kW<br>         • Base Load: 700 kW<br>         • Base Cost: 220,000,000 VND         </div>`)[0];
                popup_f4359f32f4d7bf285111773483d294c5.setContent(html_fa9f070763d323db75b648e88339407a);
            
        

        marker_b49f189ced40063eb198ed35de03d024.bindPopup(popup_f4359f32f4d7bf285111773483d294c5)
        ;

        
    
    
            marker_b49f189ced40063eb198ed35de03d024.bindTooltip(
                `<div>
                     Bệnh viện Thanh Nhàn (❌ NOT SELECTED)
                 </div>`,
                {
  "sticky": true,
}
            );
        
    
                marker_b49f189ced40063eb198ed35de03d024.setIcon(icon_ac0d2c327770a002b45bb22b2692df1f);
            
    
            var marker_93313a11aba2910ae2fb886c153a9210 = L.marker(
                [21.0027788732352, 105.861731207862],
                {
}
            ).addTo(map_c8ff09de98adc905a54fc2040c1d5971);
        
    
            var icon_42117a88413ed67f06f7432ded10fe69 = L.AwesomeMarkers.icon(
                {
  "markerColor": "red",
  "iconColor": "white",
  "icon": "times",
  "prefix": "fa",
  "extraClasses": "fa-rotate-0",
}
            );
        
    
        var popup_df07389f33cd3040121a186829904a58 = L.popup({
  "maxWidth": 350,
});

        
            
                var html_28554c88f678712b32724ecd889c13f7 = $(`<div id="html_28554c88f678712b32724ecd889c13f7" style="width: 100.0%; height: 100.0%;">         <b style='font-size:12px'>P. Kim Ngưu</b><br>         <hr style='margin:3px 0'>         <b>❌ NOT SELECTED</b><br>         ID: Site_31<br>         District: D_07<br>         <br>         <b>🏗️ Infrastructure:</b><br>         • Area: 65 m²<br>         • Grid Power: 350 kW<br>         • Base Load: 600 kW<br>         • Base Cost: 200,000,000 VND         </div>`)[0];
                popup_df07389f33cd3040121a186829904a58.setContent(html_28554c88f678712b32724ecd889c13f7);
            
        

        marker_93313a11aba2910ae2fb886c153a9210.bindPopup(popup_df07389f33cd3040121a186829904a58)
        ;

        
    
    
            marker_93313a11aba2910ae2fb886c153a9210.bindTooltip(
                `<div>
                     P. Kim Ngưu (❌ NOT SELECTED)
                 </div>`,
                {
  "sticky": true,
}
            );
        
    
                marker_93313a11aba2910ae2fb886c153a9210.setIcon(icon_42117a88413ed67f06f7432ded10fe69);
            
    
            var marker_29130ddb478c66fbdb15d58415791fef = L.marker(
                [20.9964507101763, 105.850167336697],
                {
}
            ).addTo(map_c8ff09de98adc905a54fc2040c1d5971);
        
    
            var icon_2edf867646ac0714c89eed1bb9e52803 = L.AwesomeMarkers.icon(
                {
  "markerColor": "red",
  "iconColor": "white",
  "icon": "times",
  "prefix": "fa",
  "extraClasses": "fa-rotate-0",
}
            );
        
    
        var popup_2f4d4f5e21a47f60cd6178934ac1d46c = L.popup({
  "maxWidth": 350,
});

        
            
                var html_2d57cc693352c9c4738f6621a702032e = $(`<div id="html_2d57cc693352c9c4738f6621a702032e" style="width: 100.0%; height: 100.0%;">         <b style='font-size:12px'>Chợ Mơ</b><br>         <hr style='margin:3px 0'>         <b>❌ NOT SELECTED</b><br>         ID: Site_32<br>         District: D_07<br>         <br>         <b>🏗️ Infrastructure:</b><br>         • Area: 80 m²<br>         • Grid Power: 500 kW<br>         • Base Load: 900 kW<br>         • Base Cost: 250,000,000 VND         </div>`)[0];
                popup_2f4d4f5e21a47f60cd6178934ac1d46c.setContent(html_2d57cc693352c9c4738f6621a702032e);
            
        

        marker_29130ddb478c66fbdb15d58415791fef.bindPopup(popup_2f4d4f5e21a47f60cd6178934ac1d46c)
        ;

        
    
    
            marker_29130ddb478c66fbdb15d58415791fef.bindTooltip(
                `<div>
                     Chợ Mơ (❌ NOT SELECTED)
                 </div>`,
                {
  "sticky": true,
}
            );
        
    
                marker_29130ddb478c66fbdb15d58415791fef.setIcon(icon_2edf867646ac0714c89eed1bb9e52803);
            
    
            var marker_6d05676032c49e607aea6663cce5d37c = L.marker(
                [20.967999474924, 105.826531384399],
                {
}
            ).addTo(map_c8ff09de98adc905a54fc2040c1d5971);
        
    
            var icon_6198fce652fc5ef92a5b6bdb1c3d5d45 = L.AwesomeMarkers.icon(
                {
  "markerColor": "red",
  "iconColor": "white",
  "icon": "times",
  "prefix": "fa",
  "extraClasses": "fa-rotate-0",
}
            );
        
    
        var popup_6b13da7c4d553c9122fc56fa0b128a3c = L.popup({
  "maxWidth": 350,
});

        
            
                var html_c439311f083c730c0f39258f8212a0f5 = $(`<div id="html_c439311f083c730c0f39258f8212a0f5" style="width: 100.0%; height: 100.0%;">         <b style='font-size:12px'>Bãi xe khu đô thị Linh Đàm</b><br>         <hr style='margin:3px 0'>         <b>❌ NOT SELECTED</b><br>         ID: Site_33<br>         District: D_08<br>         <br>         <b>🏗️ Infrastructure:</b><br>         • Area: 95 m²<br>         • Grid Power: 1500 kW<br>         • Base Load: 1000 kW<br>         • Base Cost: 300,000,000 VND         </div>`)[0];
                popup_6b13da7c4d553c9122fc56fa0b128a3c.setContent(html_c439311f083c730c0f39258f8212a0f5);
            
        

        marker_6d05676032c49e607aea6663cce5d37c.bindPopup(popup_6b13da7c4d553c9122fc56fa0b128a3c)
        ;

        
    
    
            marker_6d05676032c49e607aea6663cce5d37c.bindTooltip(
                `<div>
                     Bãi xe khu đô thị Linh Đàm (❌ NOT SELECTED)
                 </div>`,
                {
  "sticky": true,
}
            );
        
    
                marker_6d05676032c49e607aea6663cce5d37c.setIcon(icon_6198fce652fc5ef92a5b6bdb1c3d5d45);
            
    
            var marker_19c9d3afb6aad5c11cc7d4a3135cebf0 = L.marker(
                [20.9659561450827, 105.8424142304],
                {
}
            ).addTo(map_c8ff09de98adc905a54fc2040c1d5971);
        
    
            var icon_63305b3e13c831cd6e1914782e0bb626 = L.AwesomeMarkers.icon(
                {
  "markerColor": "green",
  "iconColor": "white",
  "icon": "bolt",
  "prefix": "fa",
  "extraClasses": "fa-rotate-0",
}
            );
        
    
        var popup_dddaa1f412fad1d93f036e837f18103e = L.popup({
  "maxWidth": 350,
});

        
            
                var html_44847273f6739372d287790651f58537 = $(`<div id="html_44847273f6739372d287790651f58537" style="width: 100.0%; height: 100.0%;">         <b style='font-size:12px'>Bến xe Nước Ngầm</b><br>         <hr style='margin:3px 0'>         <b>✅ SELECTED</b><br>         ID: Site_34<br>         District: D_08<br>         <br>         <b>📊 Specifications:</b><br>         • Chargers: <b>9</b> ports<br>         • Power: <b>1350</b> kW<br>         • Output: <b>7,800</b> kWh/day<br>         • Capital: <b>5,720,000,000</b> Million VND<br>         <br>         <b>🏗️ Infrastructure:</b><br>         • Area: 100 m²<br>         • Grid Power: 1500 kW<br>         • Base Load: 1100 kW         </div>`)[0];
                popup_dddaa1f412fad1d93f036e837f18103e.setContent(html_44847273f6739372d287790651f58537);
            
        

        marker_19c9d3afb6aad5c11cc7d4a3135cebf0.bindPopup(popup_dddaa1f412fad1d93f036e837f18103e)
        ;

        
    
    
            marker_19c9d3afb6aad5c11cc7d4a3135cebf0.bindTooltip(
                `<div>
                     Bến xe Nước Ngầm (✅ SELECTED)
                 </div>`,
                {
  "sticky": true,
}
            );
        
    
                marker_19c9d3afb6aad5c11cc7d4a3135cebf0.setIcon(icon_63305b3e13c831cd6e1914782e0bb626);
            
    
            var marker_23cd245039ee7571c0efbc63ca0594b2 = L.marker(
                [20.9834906852909, 105.85757955389],
                {
}
            ).addTo(map_c8ff09de98adc905a54fc2040c1d5971);
        
    
            var icon_09fb6ad2f21d89a48230b8339a89707f = L.AwesomeMarkers.icon(
                {
  "markerColor": "green",
  "iconColor": "white",
  "icon": "bolt",
  "prefix": "fa",
  "extraClasses": "fa-rotate-0",
}
            );
        
    
        var popup_ee63ffad42e44cd2ef2bb88045674bf8 = L.popup({
  "maxWidth": 350,
});

        
            
                var html_019ceeb1fba711f651e468630c94fdb4 = $(`<div id="html_019ceeb1fba711f651e468630c94fdb4" style="width: 100.0%; height: 100.0%;">         <b style='font-size:12px'>Đền Lừ</b><br>         <hr style='margin:3px 0'>         <b>✅ SELECTED</b><br>         ID: Site_35<br>         District: D_08<br>         <br>         <b>📊 Specifications:</b><br>         • Chargers: <b>8</b> ports<br>         • Power: <b>1200</b> kW<br>         • Output: <b>5,760</b> kWh/day<br>         • Capital: <b>5,080,000,000</b> Million VND<br>         <br>         <b>🏗️ Infrastructure:</b><br>         • Area: 85 m²<br>         • Grid Power: 1200 kW<br>         • Base Load: 900 kW         </div>`)[0];
                popup_ee63ffad42e44cd2ef2bb88045674bf8.setContent(html_019ceeb1fba711f651e468630c94fdb4);
            
        

        marker_23cd245039ee7571c0efbc63ca0594b2.bindPopup(popup_ee63ffad42e44cd2ef2bb88045674bf8)
        ;

        
    
    
            marker_23cd245039ee7571c0efbc63ca0594b2.bindTooltip(
                `<div>
                     Đền Lừ (✅ SELECTED)
                 </div>`,
                {
  "sticky": true,
}
            );
        
    
                marker_23cd245039ee7571c0efbc63ca0594b2.setIcon(icon_09fb6ad2f21d89a48230b8339a89707f);
            
    
            var marker_cd2992d1a1e422de2f7a743aa470deb7 = L.marker(
                [20.9646313273372, 105.854585521353],
                {
}
            ).addTo(map_c8ff09de98adc905a54fc2040c1d5971);
        
    
            var icon_18ed817925df8cb5ab575dd4b436f70a = L.AwesomeMarkers.icon(
                {
  "markerColor": "red",
  "iconColor": "white",
  "icon": "times",
  "prefix": "fa",
  "extraClasses": "fa-rotate-0",
}
            );
        
    
        var popup_5fcbecc03c35c31b3238ce49fd2d79a4 = L.popup({
  "maxWidth": 350,
});

        
            
                var html_ac19a8041c494c99bdf7c04d9ff73ffb = $(`<div id="html_ac19a8041c494c99bdf7c04d9ff73ffb" style="width: 100.0%; height: 100.0%;">         <b style='font-size:12px'>Công viên Yên Sở</b><br>         <hr style='margin:3px 0'>         <b>❌ NOT SELECTED</b><br>         ID: Site_36<br>         District: D_08<br>         <br>         <b>🏗️ Infrastructure:</b><br>         • Area: 100 m²<br>         • Grid Power: 2000 kW<br>         • Base Load: 1200 kW<br>         • Base Cost: 350,000,000 VND         </div>`)[0];
                popup_5fcbecc03c35c31b3238ce49fd2d79a4.setContent(html_ac19a8041c494c99bdf7c04d9ff73ffb);
            
        

        marker_cd2992d1a1e422de2f7a743aa470deb7.bindPopup(popup_5fcbecc03c35c31b3238ce49fd2d79a4)
        ;

        
    
    
            marker_cd2992d1a1e422de2f7a743aa470deb7.bindTooltip(
                `<div>
                     Công viên Yên Sở (❌ NOT SELECTED)
                 </div>`,
                {
  "sticky": true,
}
            );
        
    
                marker_cd2992d1a1e422de2f7a743aa470deb7.setIcon(icon_18ed817925df8cb5ab575dd4b436f70a);
            
    
            var marker_5166b9d2106bd1dfa8a594cc2cdce773 = L.marker(
                [20.9853406429572, 105.84671735574],
                {
}
            ).addTo(map_c8ff09de98adc905a54fc2040c1d5971);
        
    
            var icon_6540bdd7aeee829574dc09ecfe8127cd = L.AwesomeMarkers.icon(
                {
  "markerColor": "red",
  "iconColor": "white",
  "icon": "times",
  "prefix": "fa",
  "extraClasses": "fa-rotate-0",
}
            );
        
    
        var popup_4b66dfa5c9a7121c4b11e1468f4ecc58 = L.popup({
  "maxWidth": 350,
});

        
            
                var html_a88d5453381fcb769b50f390a40904a2 = $(`<div id="html_a88d5453381fcb769b50f390a40904a2" style="width: 100.0%; height: 100.0%;">         <b style='font-size:12px'>Trương Định Plaza</b><br>         <hr style='margin:3px 0'>         <b>❌ NOT SELECTED</b><br>         ID: Site_37<br>         District: D_08<br>         <br>         <b>🏗️ Infrastructure:</b><br>         • Area: 80 m²<br>         • Grid Power: 1200 kW<br>         • Base Load: 950 kW<br>         • Base Cost: 300,000,000 VND         </div>`)[0];
                popup_4b66dfa5c9a7121c4b11e1468f4ecc58.setContent(html_a88d5453381fcb769b50f390a40904a2);
            
        

        marker_5166b9d2106bd1dfa8a594cc2cdce773.bindPopup(popup_4b66dfa5c9a7121c4b11e1468f4ecc58)
        ;

        
    
    
            marker_5166b9d2106bd1dfa8a594cc2cdce773.bindTooltip(
                `<div>
                     Trương Định Plaza (❌ NOT SELECTED)
                 </div>`,
                {
  "sticky": true,
}
            );
        
    
                marker_5166b9d2106bd1dfa8a594cc2cdce773.setIcon(icon_6540bdd7aeee829574dc09ecfe8127cd);
            
    
            var marker_230e83a44550f779871f328527e1a7c6 = L.marker(
                [20.9645698744618, 105.822642055303],
                {
}
            ).addTo(map_c8ff09de98adc905a54fc2040c1d5971);
        
    
            var icon_d71140e589b0008f193280746f88c767 = L.AwesomeMarkers.icon(
                {
  "markerColor": "red",
  "iconColor": "white",
  "icon": "times",
  "prefix": "fa",
  "extraClasses": "fa-rotate-0",
}
            );
        
    
        var popup_ca633a37deee796cdcbc7baf67299f24 = L.popup({
  "maxWidth": 350,
});

        
            
                var html_7740eeec0b7ac0891d4091e1d3a7cd65 = $(`<div id="html_7740eeec0b7ac0891d4091e1d3a7cd65" style="width: 100.0%; height: 100.0%;">         <b style='font-size:12px'>Rice City</b><br>         <hr style='margin:3px 0'>         <b>❌ NOT SELECTED</b><br>         ID: Site_38<br>         District: D_08<br>         <br>         <b>🏗️ Infrastructure:</b><br>         • Area: 75 m²<br>         • Grid Power: 1000 kW<br>         • Base Load: 850 kW<br>         • Base Cost: 280,000,000 VND         </div>`)[0];
                popup_ca633a37deee796cdcbc7baf67299f24.setContent(html_7740eeec0b7ac0891d4091e1d3a7cd65);
            
        

        marker_230e83a44550f779871f328527e1a7c6.bindPopup(popup_ca633a37deee796cdcbc7baf67299f24)
        ;

        
    
    
            marker_230e83a44550f779871f328527e1a7c6.bindTooltip(
                `<div>
                     Rice City (❌ NOT SELECTED)
                 </div>`,
                {
  "sticky": true,
}
            );
        
    
                marker_230e83a44550f779871f328527e1a7c6.setIcon(icon_d71140e589b0008f193280746f88c767);
            
    
            var marker_44700b15946f2c45142a56b3b58b2f7b = L.marker(
                [20.9749409928213, 105.825652609285],
                {
}
            ).addTo(map_c8ff09de98adc905a54fc2040c1d5971);
        
    
            var icon_440cc7e3da7eb5dea4859dbe127a308a = L.AwesomeMarkers.icon(
                {
  "markerColor": "red",
  "iconColor": "white",
  "icon": "times",
  "prefix": "fa",
  "extraClasses": "fa-rotate-0",
}
            );
        
    
        var popup_2417a4f0359bc9b4e23f092c1e555113 = L.popup({
  "maxWidth": 350,
});

        
            
                var html_78703299ea492912e72caae20024c5a7 = $(`<div id="html_78703299ea492912e72caae20024c5a7" style="width: 100.0%; height: 100.0%;">         <b style='font-size:12px'>Chung cư Đại Kim</b><br>         <hr style='margin:3px 0'>         <b>❌ NOT SELECTED</b><br>         ID: Site_39<br>         District: D_08<br>         <br>         <b>🏗️ Infrastructure:</b><br>         • Area: 70 m²<br>         • Grid Power: 1000 kW<br>         • Base Load: 800 kW<br>         • Base Cost: 260,000,000 VND         </div>`)[0];
                popup_2417a4f0359bc9b4e23f092c1e555113.setContent(html_78703299ea492912e72caae20024c5a7);
            
        

        marker_44700b15946f2c45142a56b3b58b2f7b.bindPopup(popup_2417a4f0359bc9b4e23f092c1e555113)
        ;

        
    
    
            marker_44700b15946f2c45142a56b3b58b2f7b.bindTooltip(
                `<div>
                     Chung cư Đại Kim (❌ NOT SELECTED)
                 </div>`,
                {
  "sticky": true,
}
            );
        
    
                marker_44700b15946f2c45142a56b3b58b2f7b.setIcon(icon_440cc7e3da7eb5dea4859dbe127a308a);
            
    
            var marker_d440f326e39957b309d2ecfe725fa50a = L.marker(
                [20.9811157015231, 105.841989999697],
                {
}
            ).addTo(map_c8ff09de98adc905a54fc2040c1d5971);
        
    
            var icon_6f7b3be33ea4d0f6cec4015bfece332d = L.AwesomeMarkers.icon(
                {
  "markerColor": "red",
  "iconColor": "white",
  "icon": "times",
  "prefix": "fa",
  "extraClasses": "fa-rotate-0",
}
            );
        
    
        var popup_771bfddb12d4381c3f6d90dfde2e8012 = L.popup({
  "maxWidth": 350,
});

        
            
                var html_396c86fe331e2688df9745711d9703a3 = $(`<div id="html_396c86fe331e2688df9745711d9703a3" style="width: 100.0%; height: 100.0%;">         <b style='font-size:12px'>Bến xe Giáp Bát</b><br>         <hr style='margin:3px 0'>         <b>❌ NOT SELECTED</b><br>         ID: Site_40<br>         District: D_08<br>         <br>         <b>🏗️ Infrastructure:</b><br>         • Area: 100 m²<br>         • Grid Power: 1500 kW<br>         • Base Load: 1100 kW<br>         • Base Cost: 320,000,000 VND         </div>`)[0];
                popup_771bfddb12d4381c3f6d90dfde2e8012.setContent(html_396c86fe331e2688df9745711d9703a3);
            
        

        marker_d440f326e39957b309d2ecfe725fa50a.bindPopup(popup_771bfddb12d4381c3f6d90dfde2e8012)
        ;

        
    
    
            marker_d440f326e39957b309d2ecfe725fa50a.bindTooltip(
                `<div>
                     Bến xe Giáp Bát (❌ NOT SELECTED)
                 </div>`,
                {
  "sticky": true,
}
            );
        
    
                marker_d440f326e39957b309d2ecfe725fa50a.setIcon(icon_6f7b3be33ea4d0f6cec4015bfece332d);
            
    
            var marker_9280a5f457be8c5faaae181efe1f406e = L.marker(
                [21.0033551688671, 105.815410579026],
                {
}
            ).addTo(map_c8ff09de98adc905a54fc2040c1d5971);
        
    
            var icon_f0ccee8d31a39d9fd01ba658bc72ef94 = L.AwesomeMarkers.icon(
                {
  "markerColor": "red",
  "iconColor": "white",
  "icon": "times",
  "prefix": "fa",
  "extraClasses": "fa-rotate-0",
}
            );
        
    
        var popup_54b734fef257cb50494268b65104ff07 = L.popup({
  "maxWidth": 350,
});

        
            
                var html_4352160157a5a8a55c30b642bf24dddb = $(`<div id="html_4352160157a5a8a55c30b642bf24dddb" style="width: 100.0%; height: 100.0%;">         <b style='font-size:12px'>Royal City</b><br>         <hr style='margin:3px 0'>         <b>❌ NOT SELECTED</b><br>         ID: Site_41<br>         District: D_09<br>         <br>         <b>🏗️ Infrastructure:</b><br>         • Area: 100 m²<br>         • Grid Power: 2000 kW<br>         • Base Load: 1200 kW<br>         • Base Cost: 350,000,000 VND         </div>`)[0];
                popup_54b734fef257cb50494268b65104ff07.setContent(html_4352160157a5a8a55c30b642bf24dddb);
            
        

        marker_9280a5f457be8c5faaae181efe1f406e.bindPopup(popup_54b734fef257cb50494268b65104ff07)
        ;

        
    
    
            marker_9280a5f457be8c5faaae181efe1f406e.bindTooltip(
                `<div>
                     Royal City (❌ NOT SELECTED)
                 </div>`,
                {
  "sticky": true,
}
            );
        
    
                marker_9280a5f457be8c5faaae181efe1f406e.setIcon(icon_f0ccee8d31a39d9fd01ba658bc72ef94);
            
    
            var marker_571a1a42b8f1dc2a2990a5613b94d545 = L.marker(
                [20.9988674508698, 105.796473057468],
                {
}
            ).addTo(map_c8ff09de98adc905a54fc2040c1d5971);
        
    
            var icon_838798fa0a21290874c30c35228b4fcf = L.AwesomeMarkers.icon(
                {
  "markerColor": "red",
  "iconColor": "white",
  "icon": "times",
  "prefix": "fa",
  "extraClasses": "fa-rotate-0",
}
            );
        
    
        var popup_69833ac53d4ea043664b291508e3f591 = L.popup({
  "maxWidth": 350,
});

        
            
                var html_be6dcc71eb7c738256f41ea1f413ebc6 = $(`<div id="html_be6dcc71eb7c738256f41ea1f413ebc6" style="width: 100.0%; height: 100.0%;">         <b style='font-size:12px'>Bãi Đậu Xe 24/7</b><br>         <hr style='margin:3px 0'>         <b>❌ NOT SELECTED</b><br>         ID: Site_42<br>         District: D_09<br>         <br>         <b>🏗️ Infrastructure:</b><br>         • Area: 80 m²<br>         • Grid Power: 1000 kW<br>         • Base Load: 800 kW<br>         • Base Cost: 260,000,000 VND         </div>`)[0];
                popup_69833ac53d4ea043664b291508e3f591.setContent(html_be6dcc71eb7c738256f41ea1f413ebc6);
            
        

        marker_571a1a42b8f1dc2a2990a5613b94d545.bindPopup(popup_69833ac53d4ea043664b291508e3f591)
        ;

        
    
    
            marker_571a1a42b8f1dc2a2990a5613b94d545.bindTooltip(
                `<div>
                     Bãi Đậu Xe 24/7 (❌ NOT SELECTED)
                 </div>`,
                {
  "sticky": true,
}
            );
        
    
                marker_571a1a42b8f1dc2a2990a5613b94d545.setIcon(icon_838798fa0a21290874c30c35228b4fcf);
            
    
            var marker_52e09b4f2ab34c4526a772e2f22aaaab = L.marker(
                [20.9871406789402, 105.796355008673],
                {
}
            ).addTo(map_c8ff09de98adc905a54fc2040c1d5971);
        
    
            var icon_72c9807d85b0fa2f1b7b4d4f36281862 = L.AwesomeMarkers.icon(
                {
  "markerColor": "red",
  "iconColor": "white",
  "icon": "times",
  "prefix": "fa",
  "extraClasses": "fa-rotate-0",
}
            );
        
    
        var popup_d8d768237f6633aeef9d22ced9b84216 = L.popup({
  "maxWidth": 350,
});

        
            
                var html_0227bed75434f7218088481ce8cc08fa = $(`<div id="html_0227bed75434f7218088481ce8cc08fa" style="width: 100.0%; height: 100.0%;">         <b style='font-size:12px'>Bãi đỗ xe Phùng Khoang</b><br>         <hr style='margin:3px 0'>         <b>❌ NOT SELECTED</b><br>         ID: Site_43<br>         District: D_09<br>         <br>         <b>🏗️ Infrastructure:</b><br>         • Area: 70 m²<br>         • Grid Power: 1000 kW<br>         • Base Load: 750 kW<br>         • Base Cost: 250,000,000 VND         </div>`)[0];
                popup_d8d768237f6633aeef9d22ced9b84216.setContent(html_0227bed75434f7218088481ce8cc08fa);
            
        

        marker_52e09b4f2ab34c4526a772e2f22aaaab.bindPopup(popup_d8d768237f6633aeef9d22ced9b84216)
        ;

        
    
    
            marker_52e09b4f2ab34c4526a772e2f22aaaab.bindTooltip(
                `<div>
                     Bãi đỗ xe Phùng Khoang (❌ NOT SELECTED)
                 </div>`,
                {
  "sticky": true,
}
            );
        
    
                marker_52e09b4f2ab34c4526a772e2f22aaaab.setIcon(icon_72c9807d85b0fa2f1b7b4d4f36281862);
            
    
            var marker_1a373d2474965bba0ebd9dfc59f82625 = L.marker(
                [21.0019411811774, 105.823011757468],
                {
}
            ).addTo(map_c8ff09de98adc905a54fc2040c1d5971);
        
    
            var icon_435f95e3e167d1e74d94a1679b2d5404 = L.AwesomeMarkers.icon(
                {
  "markerColor": "red",
  "iconColor": "white",
  "icon": "times",
  "prefix": "fa",
  "extraClasses": "fa-rotate-0",
}
            );
        
    
        var popup_4c83d57945db42e54f447ea7f8519eba = L.popup({
  "maxWidth": 350,
});

        
            
                var html_2d89e4771284e58a31b85b23b28e9686 = $(`<div id="html_2d89e4771284e58a31b85b23b28e9686" style="width: 100.0%; height: 100.0%;">         <b style='font-size:12px'>Bãi đỗ xe Trường Chinh</b><br>         <hr style='margin:3px 0'>         <b>❌ NOT SELECTED</b><br>         ID: Site_44<br>         District: D_09<br>         <br>         <b>🏗️ Infrastructure:</b><br>         • Area: 80 m²<br>         • Grid Power: 1200 kW<br>         • Base Load: 900 kW<br>         • Base Cost: 280,000,000 VND         </div>`)[0];
                popup_4c83d57945db42e54f447ea7f8519eba.setContent(html_2d89e4771284e58a31b85b23b28e9686);
            
        

        marker_1a373d2474965bba0ebd9dfc59f82625.bindPopup(popup_4c83d57945db42e54f447ea7f8519eba)
        ;

        
    
    
            marker_1a373d2474965bba0ebd9dfc59f82625.bindTooltip(
                `<div>
                     Bãi đỗ xe Trường Chinh (❌ NOT SELECTED)
                 </div>`,
                {
  "sticky": true,
}
            );
        
    
                marker_1a373d2474965bba0ebd9dfc59f82625.setIcon(icon_435f95e3e167d1e74d94a1679b2d5404);
            
    
            var marker_96c9381721b8cdfb9ec02c447577ec79 = L.marker(
                [21.0030219494811, 105.797524438121],
                {
}
            ).addTo(map_c8ff09de98adc905a54fc2040c1d5971);
        
    
            var icon_d06070aea1b38ebd363510d20e146800 = L.AwesomeMarkers.icon(
                {
  "markerColor": "red",
  "iconColor": "white",
  "icon": "times",
  "prefix": "fa",
  "extraClasses": "fa-rotate-0",
}
            );
        
    
        var popup_586da727cea9d38102872237bb9d3df6 = L.popup({
  "maxWidth": 350,
});

        
            
                var html_5c5645042f30e3185116c4e3b0be192b = $(`<div id="html_5c5645042f30e3185116c4e3b0be192b" style="width: 100.0%; height: 100.0%;">         <b style='font-size:12px'>Công viên hồ điều hòa Nhân Chính</b><br>         <hr style='margin:3px 0'>         <b>❌ NOT SELECTED</b><br>         ID: Site_45<br>         District: D_09<br>         <br>         <b>🏗️ Infrastructure:</b><br>         • Area: 75 m²<br>         • Grid Power: 1000 kW<br>         • Base Load: 800 kW<br>         • Base Cost: 260,000,000 VND         </div>`)[0];
                popup_586da727cea9d38102872237bb9d3df6.setContent(html_5c5645042f30e3185116c4e3b0be192b);
            
        

        marker_96c9381721b8cdfb9ec02c447577ec79.bindPopup(popup_586da727cea9d38102872237bb9d3df6)
        ;

        
    
    
            marker_96c9381721b8cdfb9ec02c447577ec79.bindTooltip(
                `<div>
                     Công viên hồ điều hòa Nhân Chính (❌ NOT SELECTED)
                 </div>`,
                {
  "sticky": true,
}
            );
        
    
                marker_96c9381721b8cdfb9ec02c447577ec79.setIcon(icon_d06070aea1b38ebd363510d20e146800);
            
    
            var marker_7d82b8e756fec4f491a6bdbbfe5f0b68 = L.marker(
                [20.9998415381356, 105.807610136275],
                {
}
            ).addTo(map_c8ff09de98adc905a54fc2040c1d5971);
        
    
            var icon_c7b05e6bb23107e3b575a5ba81b6c622 = L.AwesomeMarkers.icon(
                {
  "markerColor": "red",
  "iconColor": "white",
  "icon": "times",
  "prefix": "fa",
  "extraClasses": "fa-rotate-0",
}
            );
        
    
        var popup_32e1efddcf64d965c5524f069df78d40 = L.popup({
  "maxWidth": 350,
});

        
            
                var html_909063292fd011368e0cd4e09a17460e = $(`<div id="html_909063292fd011368e0cd4e09a17460e" style="width: 100.0%; height: 100.0%;">         <b style='font-size:12px'>Hapulico Complex</b><br>         <hr style='margin:3px 0'>         <b>❌ NOT SELECTED</b><br>         ID: Site_46<br>         District: D_09<br>         <br>         <b>🏗️ Infrastructure:</b><br>         • Area: 90 m²<br>         • Grid Power: 1200 kW<br>         • Base Load: 950 kW<br>         • Base Cost: 300,000,000 VND         </div>`)[0];
                popup_32e1efddcf64d965c5524f069df78d40.setContent(html_909063292fd011368e0cd4e09a17460e);
            
        

        marker_7d82b8e756fec4f491a6bdbbfe5f0b68.bindPopup(popup_32e1efddcf64d965c5524f069df78d40)
        ;

        
    
    
            marker_7d82b8e756fec4f491a6bdbbfe5f0b68.bindTooltip(
                `<div>
                     Hapulico Complex (❌ NOT SELECTED)
                 </div>`,
                {
  "sticky": true,
}
            );
        
    
                marker_7d82b8e756fec4f491a6bdbbfe5f0b68.setIcon(icon_c7b05e6bb23107e3b575a5ba81b6c622);
            
    
            var marker_0ca06a8a9a77cde85e964e44ac38cca5 = L.marker(
                [20.995556528672, 105.804596378605],
                {
}
            ).addTo(map_c8ff09de98adc905a54fc2040c1d5971);
        
    
            var icon_b4d04f32c7c36e95251f65a957b1ea71 = L.AwesomeMarkers.icon(
                {
  "markerColor": "red",
  "iconColor": "white",
  "icon": "times",
  "prefix": "fa",
  "extraClasses": "fa-rotate-0",
}
            );
        
    
        var popup_73ea0deef83469d3afc1d170062e04fc = L.popup({
  "maxWidth": 350,
});

        
            
                var html_0aa44db1e668d4c86cd66920da007f65 = $(`<div id="html_0aa44db1e668d4c86cd66920da007f65" style="width: 100.0%; height: 100.0%;">         <b style='font-size:12px'>Goldseason</b><br>         <hr style='margin:3px 0'>         <b>❌ NOT SELECTED</b><br>         ID: Site_47<br>         District: D_09<br>         <br>         <b>🏗️ Infrastructure:</b><br>         • Area: 90 m²<br>         • Grid Power: 1200 kW<br>         • Base Load: 950 kW<br>         • Base Cost: 300,000,000 VND         </div>`)[0];
                popup_73ea0deef83469d3afc1d170062e04fc.setContent(html_0aa44db1e668d4c86cd66920da007f65);
            
        

        marker_0ca06a8a9a77cde85e964e44ac38cca5.bindPopup(popup_73ea0deef83469d3afc1d170062e04fc)
        ;

        
    
    
            marker_0ca06a8a9a77cde85e964e44ac38cca5.bindTooltip(
                `<div>
                     Goldseason (❌ NOT SELECTED)
                 </div>`,
                {
  "sticky": true,
}
            );
        
    
                marker_0ca06a8a9a77cde85e964e44ac38cca5.setIcon(icon_b4d04f32c7c36e95251f65a957b1ea71);
            
    
            var marker_6a70d51d00aa17fd1428fe6126711c65 = L.marker(
                [20.9804716313407, 105.814821769484],
                {
}
            ).addTo(map_c8ff09de98adc905a54fc2040c1d5971);
        
    
            var icon_c44be28ae9969a9e620e2f09efbf630f = L.AwesomeMarkers.icon(
                {
  "markerColor": "green",
  "iconColor": "white",
  "icon": "bolt",
  "prefix": "fa",
  "extraClasses": "fa-rotate-0",
}
            );
        
    
        var popup_3bba5920de985505dd06acb122426868 = L.popup({
  "maxWidth": 350,
});

        
            
                var html_d70df65124d87122ea687e0a4e09ca6f = $(`<div id="html_d70df65124d87122ea687e0a4e09ca6f" style="width: 100.0%; height: 100.0%;">         <b style='font-size:12px'>Bãi đỗ xe Kim Giang</b><br>         <hr style='margin:3px 0'>         <b>✅ SELECTED</b><br>         ID: Site_48<br>         District: D_09<br>         <br>         <b>📊 Specifications:</b><br>         • Chargers: <b>7</b> ports<br>         • Power: <b>1050</b> kW<br>         • Output: <b>4,800</b> kWh/day<br>         • Capital: <b>4,450,000,000</b> Million VND<br>         <br>         <b>🏗️ Infrastructure:</b><br>         • Area: 70 m²<br>         • Grid Power: 1000 kW<br>         • Base Load: 750 kW         </div>`)[0];
                popup_3bba5920de985505dd06acb122426868.setContent(html_d70df65124d87122ea687e0a4e09ca6f);
            
        

        marker_6a70d51d00aa17fd1428fe6126711c65.bindPopup(popup_3bba5920de985505dd06acb122426868)
        ;

        
    
    
            marker_6a70d51d00aa17fd1428fe6126711c65.bindTooltip(
                `<div>
                     Bãi đỗ xe Kim Giang (✅ SELECTED)
                 </div>`,
                {
  "sticky": true,
}
            );
        
    
                marker_6a70d51d00aa17fd1428fe6126711c65.setIcon(icon_c44be28ae9969a9e620e2f09efbf630f);
            
    
            var marker_111987d43e2e7d0ef1ad3f190b1a8d60 = L.marker(
                [21.0072439672541, 105.795750526984],
                {
}
            ).addTo(map_c8ff09de98adc905a54fc2040c1d5971);
        
    
            var icon_24487bc7c70da498ad3565edad11d1e1 = L.AwesomeMarkers.icon(
                {
  "markerColor": "red",
  "iconColor": "white",
  "icon": "times",
  "prefix": "fa",
  "extraClasses": "fa-rotate-0",
}
            );
        
    
        var popup_3d74ad63749f1a39fa421128b46bce92 = L.popup({
  "maxWidth": 350,
});

        
            
                var html_7f2f4e329171954d5460a08b01a78731 = $(`<div id="html_7f2f4e329171954d5460a08b01a78731" style="width: 100.0%; height: 100.0%;">         <b style='font-size:12px'>Vincom Center Trần Duy Hưng</b><br>         <hr style='margin:3px 0'>         <b>❌ NOT SELECTED</b><br>         ID: Site_49<br>         District: D_05<br>         <br>         <b>🏗️ Infrastructure:</b><br>         • Area: 100 m²<br>         • Grid Power: 1500 kW<br>         • Base Load: 1200 kW<br>         • Base Cost: 300,000,000 VND         </div>`)[0];
                popup_3d74ad63749f1a39fa421128b46bce92.setContent(html_7f2f4e329171954d5460a08b01a78731);
            
        

        marker_111987d43e2e7d0ef1ad3f190b1a8d60.bindPopup(popup_3d74ad63749f1a39fa421128b46bce92)
        ;

        
    
    
            marker_111987d43e2e7d0ef1ad3f190b1a8d60.bindTooltip(
                `<div>
                     Vincom Center Trần Duy Hưng (❌ NOT SELECTED)
                 </div>`,
                {
  "sticky": true,
}
            );
        
    
                marker_111987d43e2e7d0ef1ad3f190b1a8d60.setIcon(icon_24487bc7c70da498ad3565edad11d1e1);
            
    
            var marker_832e5a8df64b158fcae2284f69ad00af = L.marker(
                [21.0075594201988, 105.793187999999],
                {
}
            ).addTo(map_c8ff09de98adc905a54fc2040c1d5971);
        
    
            var icon_23c9dcd84d1086bdeff00907efdcb9ca = L.AwesomeMarkers.icon(
                {
  "markerColor": "red",
  "iconColor": "white",
  "icon": "times",
  "prefix": "fa",
  "extraClasses": "fa-rotate-0",
}
            );
        
    
        var popup_26b1f885c67688081bef51cb46917e0b = L.popup({
  "maxWidth": 350,
});

        
            
                var html_abef7865776ef5d4a0ef393a19dd9dd5 = $(`<div id="html_abef7865776ef5d4a0ef393a19dd9dd5" style="width: 100.0%; height: 100.0%;">         <b style='font-size:12px'>Big C Thăng Long</b><br>         <hr style='margin:3px 0'>         <b>❌ NOT SELECTED</b><br>         ID: Site_50<br>         District: D_05<br>         <br>         <b>🏗️ Infrastructure:</b><br>         • Area: 100 m²<br>         • Grid Power: 1400 kW<br>         • Base Load: 1100 kW<br>         • Base Cost: 280,000,000 VND         </div>`)[0];
                popup_26b1f885c67688081bef51cb46917e0b.setContent(html_abef7865776ef5d4a0ef393a19dd9dd5);
            
        

        marker_832e5a8df64b158fcae2284f69ad00af.bindPopup(popup_26b1f885c67688081bef51cb46917e0b)
        ;

        
    
    
            marker_832e5a8df64b158fcae2284f69ad00af.bindTooltip(
                `<div>
                     Big C Thăng Long (❌ NOT SELECTED)
                 </div>`,
                {
  "sticky": true,
}
            );
        
    
                marker_832e5a8df64b158fcae2284f69ad00af.setIcon(icon_23c9dcd84d1086bdeff00907efdcb9ca);
            
    
            var marker_f000f0b2f2f850268faccb1a26738a2a = L.marker(
                [21.0359688870967, 105.782779257671],
                {
}
            ).addTo(map_c8ff09de98adc905a54fc2040c1d5971);
        
    
            var icon_966ad09b0dfcfdaa5a0842da70a331ac = L.AwesomeMarkers.icon(
                {
  "markerColor": "red",
  "iconColor": "white",
  "icon": "times",
  "prefix": "fa",
  "extraClasses": "fa-rotate-0",
}
            );
        
    
        var popup_20ab61203130bba41b25c9c3e874faea = L.popup({
  "maxWidth": 350,
});

        
            
                var html_9549aee5acf0dd4e1e4681a55b38d10b = $(`<div id="html_9549aee5acf0dd4e1e4681a55b38d10b" style="width: 100.0%; height: 100.0%;">         <b style='font-size:12px'>Indochina Plaza Hà Nội</b><br>         <hr style='margin:3px 0'>         <b>❌ NOT SELECTED</b><br>         ID: Site_51<br>         District: D_05<br>         <br>         <b>🏗️ Infrastructure:</b><br>         • Area: 80 m²<br>         • Grid Power: 1300 kW<br>         • Base Load: 1050 kW<br>         • Base Cost: 280,000,000 VND         </div>`)[0];
                popup_20ab61203130bba41b25c9c3e874faea.setContent(html_9549aee5acf0dd4e1e4681a55b38d10b);
            
        

        marker_f000f0b2f2f850268faccb1a26738a2a.bindPopup(popup_20ab61203130bba41b25c9c3e874faea)
        ;

        
    
    
            marker_f000f0b2f2f850268faccb1a26738a2a.bindTooltip(
                `<div>
                     Indochina Plaza Hà Nội (❌ NOT SELECTED)
                 </div>`,
                {
  "sticky": true,
}
            );
        
    
                marker_f000f0b2f2f850268faccb1a26738a2a.setIcon(icon_966ad09b0dfcfdaa5a0842da70a331ac);
            
    
            var marker_58cbe95711a9b5d33ba4744c94919eea = L.marker(
                [21.0119845086685, 105.800458784656],
                {
}
            ).addTo(map_c8ff09de98adc905a54fc2040c1d5971);
        
    
            var icon_9b2814a157a58b4b1e7a54de599625a1 = L.AwesomeMarkers.icon(
                {
  "markerColor": "red",
  "iconColor": "white",
  "icon": "times",
  "prefix": "fa",
  "extraClasses": "fa-rotate-0",
}
            );
        
    
        var popup_d52226e2802c6ad2950a1e8aa9b20d8a = L.popup({
  "maxWidth": 350,
});

        
            
                var html_4222abed357c6e33f806a60264e0e98d = $(`<div id="html_4222abed357c6e33f806a60264e0e98d" style="width: 100.0%; height: 100.0%;">         <b style='font-size:12px'>Trần Duy Hưng Parking Complex</b><br>         <hr style='margin:3px 0'>         <b>❌ NOT SELECTED</b><br>         ID: Site_52<br>         District: D_05<br>         <br>         <b>🏗️ Infrastructure:</b><br>         • Area: 90 m²<br>         • Grid Power: 600 kW<br>         • Base Load: 250 kW<br>         • Base Cost: 200,000,000 VND         </div>`)[0];
                popup_d52226e2802c6ad2950a1e8aa9b20d8a.setContent(html_4222abed357c6e33f806a60264e0e98d);
            
        

        marker_58cbe95711a9b5d33ba4744c94919eea.bindPopup(popup_d52226e2802c6ad2950a1e8aa9b20d8a)
        ;

        
    
    
            marker_58cbe95711a9b5d33ba4744c94919eea.bindTooltip(
                `<div>
                     Trần Duy Hưng Parking Complex (❌ NOT SELECTED)
                 </div>`,
                {
  "sticky": true,
}
            );
        
    
                marker_58cbe95711a9b5d33ba4744c94919eea.setIcon(icon_9b2814a157a58b4b1e7a54de599625a1);
            
    
            var marker_8be7e6c3da0f62cb2b554ff26d421088 = L.marker(
                [21.0357202152681, 105.794687515343],
                {
}
            ).addTo(map_c8ff09de98adc905a54fc2040c1d5971);
        
    
            var icon_64d0e49bf5a3fe38c19b879a31dc15f8 = L.AwesomeMarkers.icon(
                {
  "markerColor": "red",
  "iconColor": "white",
  "icon": "times",
  "prefix": "fa",
  "extraClasses": "fa-rotate-0",
}
            );
        
    
        var popup_f12db9233a6958e2391a91a376c535d6 = L.popup({
  "maxWidth": 350,
});

        
            
                var html_f724d0a906c4b951660cc747a5f8859f = $(`<div id="html_f724d0a906c4b951660cc747a5f8859f" style="width: 100.0%; height: 100.0%;">         <b style='font-size:12px'>Chung cư Discovery Complex</b><br>         <hr style='margin:3px 0'>         <b>❌ NOT SELECTED</b><br>         ID: Site_53<br>         District: D_05<br>         <br>         <b>🏗️ Infrastructure:</b><br>         • Area: 50 m²<br>         • Grid Power: 800 kW<br>         • Base Load: 550 kW<br>         • Base Cost: 220,000,000 VND         </div>`)[0];
                popup_f12db9233a6958e2391a91a376c535d6.setContent(html_f724d0a906c4b951660cc747a5f8859f);
            
        

        marker_8be7e6c3da0f62cb2b554ff26d421088.bindPopup(popup_f12db9233a6958e2391a91a376c535d6)
        ;

        
    
    
            marker_8be7e6c3da0f62cb2b554ff26d421088.bindTooltip(
                `<div>
                     Chung cư Discovery Complex (❌ NOT SELECTED)
                 </div>`,
                {
  "sticky": true,
}
            );
        
    
                marker_8be7e6c3da0f62cb2b554ff26d421088.setIcon(icon_64d0e49bf5a3fe38c19b879a31dc15f8);
            
    
            var marker_0a42340b37b71bec5ecc9c7b522a8114 = L.marker(
                [21.0195528551574, 105.797446969312],
                {
}
            ).addTo(map_c8ff09de98adc905a54fc2040c1d5971);
        
    
            var icon_ddd8bf1aacd6af0b11435de717def930 = L.AwesomeMarkers.icon(
                {
  "markerColor": "green",
  "iconColor": "white",
  "icon": "bolt",
  "prefix": "fa",
  "extraClasses": "fa-rotate-0",
}
            );
        
    
        var popup_90e2c6ed1dfaf7b7a74c57bb44ab4306 = L.popup({
  "maxWidth": 350,
});

        
            
                var html_54fa7cbd290dab0d536e33f4cbbbe766 = $(`<div id="html_54fa7cbd290dab0d536e33f4cbbbe766" style="width: 100.0%; height: 100.0%;">         <b style='font-size:12px'>Khu đô thị Yên Hòa</b><br>         <hr style='margin:3px 0'>         <b>✅ SELECTED</b><br>         ID: Site_54<br>         District: D_05<br>         <br>         <b>📊 Specifications:</b><br>         • Chargers: <b>9</b> ports<br>         • Power: <b>1350</b> kW<br>         • Output: <b>7,200</b> kWh/day<br>         • Capital: <b>5,580,000,000</b> Million VND<br>         <br>         <b>🏗️ Infrastructure:</b><br>         • Area: 60 m²<br>         • Grid Power: 1000 kW<br>         • Base Load: 650 kW         </div>`)[0];
                popup_90e2c6ed1dfaf7b7a74c57bb44ab4306.setContent(html_54fa7cbd290dab0d536e33f4cbbbe766);
            
        

        marker_0a42340b37b71bec5ecc9c7b522a8114.bindPopup(popup_90e2c6ed1dfaf7b7a74c57bb44ab4306)
        ;

        
    
    
            marker_0a42340b37b71bec5ecc9c7b522a8114.bindTooltip(
                `<div>
                     Khu đô thị Yên Hòa (✅ SELECTED)
                 </div>`,
                {
  "sticky": true,
}
            );
        
    
                marker_0a42340b37b71bec5ecc9c7b522a8114.setIcon(icon_ddd8bf1aacd6af0b11435de717def930);
            
    
            var marker_04410cfb1fd03a9687fdb67aa107ac0a = L.marker(
                [21.038001138068, 105.782283142328],
                {
}
            ).addTo(map_c8ff09de98adc905a54fc2040c1d5971);
        
    
            var icon_a6e9326734b73fe90b4b8ba95e22fb68 = L.AwesomeMarkers.icon(
                {
  "markerColor": "red",
  "iconColor": "white",
  "icon": "times",
  "prefix": "fa",
  "extraClasses": "fa-rotate-0",
}
            );
        
    
        var popup_bf85aa0af919b9a3500da5cb94aa7486 = L.popup({
  "maxWidth": 350,
});

        
            
                var html_dbb833d3fe1bcdb35a3d0e68c4b43687 = $(`<div id="html_dbb833d3fe1bcdb35a3d0e68c4b43687" style="width: 100.0%; height: 100.0%;">         <b style='font-size:12px'>Bãi đỗ xe ĐH Quốc Gia Hà Nội</b><br>         <hr style='margin:3px 0'>         <b>❌ NOT SELECTED</b><br>         ID: Site_55<br>         District: D_05<br>         <br>         <b>🏗️ Infrastructure:</b><br>         • Area: 70 m²<br>         • Grid Power: 700 kW<br>         • Base Load: 200 kW<br>         • Base Cost: 130,000,000 VND         </div>`)[0];
                popup_bf85aa0af919b9a3500da5cb94aa7486.setContent(html_dbb833d3fe1bcdb35a3d0e68c4b43687);
            
        

        marker_04410cfb1fd03a9687fdb67aa107ac0a.bindPopup(popup_bf85aa0af919b9a3500da5cb94aa7486)
        ;

        
    
    
            marker_04410cfb1fd03a9687fdb67aa107ac0a.bindTooltip(
                `<div>
                     Bãi đỗ xe ĐH Quốc Gia Hà Nội (❌ NOT SELECTED)
                 </div>`,
                {
  "sticky": true,
}
            );
        
    
                marker_04410cfb1fd03a9687fdb67aa107ac0a.setIcon(icon_a6e9326734b73fe90b4b8ba95e22fb68);
            
    
            var marker_026790a28da075b50ed66d0317c22a48 = L.marker(
                [21.0509164102781, 105.916429742328],
                {
}
            ).addTo(map_c8ff09de98adc905a54fc2040c1d5971);
        
    
            var icon_4f67843e2a48729be6e8dde9e2f85186 = L.AwesomeMarkers.icon(
                {
  "markerColor": "red",
  "iconColor": "white",
  "icon": "times",
  "prefix": "fa",
  "extraClasses": "fa-rotate-0",
}
            );
        
    
        var popup_130f9462bd85f90a2ac9c1fb56bad96f = L.popup({
  "maxWidth": 350,
});

        
            
                var html_8a18115c00be7c4b7842b3b1f632dedb = $(`<div id="html_8a18115c00be7c4b7842b3b1f632dedb" style="width: 100.0%; height: 100.0%;">         <b style='font-size:12px'>Vincom Plaza Long Biên</b><br>         <hr style='margin:3px 0'>         <b>❌ NOT SELECTED</b><br>         ID: Site_56<br>         District: D_04<br>         <br>         <b>🏗️ Infrastructure:</b><br>         • Area: 100 m²<br>         • Grid Power: 1200 kW<br>         • Base Load: 950 kW<br>         • Base Cost: 250,000,000 VND         </div>`)[0];
                popup_130f9462bd85f90a2ac9c1fb56bad96f.setContent(html_8a18115c00be7c4b7842b3b1f632dedb);
            
        

        marker_026790a28da075b50ed66d0317c22a48.bindPopup(popup_130f9462bd85f90a2ac9c1fb56bad96f)
        ;

        
    
    
            marker_026790a28da075b50ed66d0317c22a48.bindTooltip(
                `<div>
                     Vincom Plaza Long Biên (❌ NOT SELECTED)
                 </div>`,
                {
  "sticky": true,
}
            );
        
    
                marker_026790a28da075b50ed66d0317c22a48.setIcon(icon_4f67843e2a48729be6e8dde9e2f85186);
            
    
            var marker_c89d1548a3acbb850f7cea7e71b316fe = L.marker(
                [21.0276161588911, 105.898784871164],
                {
}
            ).addTo(map_c8ff09de98adc905a54fc2040c1d5971);
        
    
            var icon_769c1c0a13fdf8623b213e57b0611752 = L.AwesomeMarkers.icon(
                {
  "markerColor": "red",
  "iconColor": "white",
  "icon": "times",
  "prefix": "fa",
  "extraClasses": "fa-rotate-0",
}
            );
        
    
        var popup_f03ed58e6293267865b936972ff0d245 = L.popup({
  "maxWidth": 350,
});

        
            
                var html_ddd24196afd047d60f5155cdfddd2613 = $(`<div id="html_ddd24196afd047d60f5155cdfddd2613" style="width: 100.0%; height: 100.0%;">         <b style='font-size:12px'>AEON Mall Long Biên</b><br>         <hr style='margin:3px 0'>         <b>❌ NOT SELECTED</b><br>         ID: Site_57<br>         District: D_04<br>         <br>         <b>🏗️ Infrastructure:</b><br>         • Area: 90 m²<br>         • Grid Power: 1500 kW<br>         • Base Load: 1200 kW<br>         • Base Cost: 300,000,000 VND         </div>`)[0];
                popup_f03ed58e6293267865b936972ff0d245.setContent(html_ddd24196afd047d60f5155cdfddd2613);
            
        

        marker_c89d1548a3acbb850f7cea7e71b316fe.bindPopup(popup_f03ed58e6293267865b936972ff0d245)
        ;

        
    
    
            marker_c89d1548a3acbb850f7cea7e71b316fe.bindTooltip(
                `<div>
                     AEON Mall Long Biên (❌ NOT SELECTED)
                 </div>`,
                {
  "sticky": true,
}
            );
        
    
                marker_c89d1548a3acbb850f7cea7e71b316fe.setIcon(icon_769c1c0a13fdf8623b213e57b0611752);
            
    
            var marker_3402447f031eb12dc69a14395dcb04df = L.marker(
                [21.0390849948569, 105.894407592328],
                {
}
            ).addTo(map_c8ff09de98adc905a54fc2040c1d5971);
        
    
            var icon_0f7a58fdb08b510f6aa186da5355b22f = L.AwesomeMarkers.icon(
                {
  "markerColor": "green",
  "iconColor": "white",
  "icon": "bolt",
  "prefix": "fa",
  "extraClasses": "fa-rotate-0",
}
            );
        
    
        var popup_27028d55e616c3fe28040e62d094bfe4 = L.popup({
  "maxWidth": 350,
});

        
            
                var html_940a1dbdde033925e01596caaacbb655 = $(`<div id="html_940a1dbdde033925e01596caaacbb655" style="width: 100.0%; height: 100.0%;">         <b style='font-size:12px'>Bãi đỗ xe Sân Golf Long Biên</b><br>         <hr style='margin:3px 0'>         <b>✅ SELECTED</b><br>         ID: Site_58<br>         District: D_04<br>         <br>         <b>📊 Specifications:</b><br>         • Chargers: <b>7</b> ports<br>         • Power: <b>1050</b> kW<br>         • Output: <b>3,809</b> kWh/day<br>         • Capital: <b>4,350,000,000</b> Million VND<br>         <br>         <b>🏗️ Infrastructure:</b><br>         • Area: 60 m²<br>         • Grid Power: 500 kW<br>         • Base Load: 200 kW         </div>`)[0];
                popup_27028d55e616c3fe28040e62d094bfe4.setContent(html_940a1dbdde033925e01596caaacbb655);
            
        

        marker_3402447f031eb12dc69a14395dcb04df.bindPopup(popup_27028d55e616c3fe28040e62d094bfe4)
        ;

        
    
    
            marker_3402447f031eb12dc69a14395dcb04df.bindTooltip(
                `<div>
                     Bãi đỗ xe Sân Golf Long Biên (✅ SELECTED)
                 </div>`,
                {
  "sticky": true,
}
            );
        
    
                marker_3402447f031eb12dc69a14395dcb04df.setIcon(icon_0f7a58fdb08b510f6aa186da5355b22f);
            
    
            var marker_37a9e816cbe54ad4458f989295bb4a4d = L.marker(
                [21.0411462099288, 105.917765157671],
                {
}
            ).addTo(map_c8ff09de98adc905a54fc2040c1d5971);
        
    
            var icon_44b27971918149696bb29828de1519e6 = L.AwesomeMarkers.icon(
                {
  "markerColor": "red",
  "iconColor": "white",
  "icon": "times",
  "prefix": "fa",
  "extraClasses": "fa-rotate-0",
}
            );
        
    
        var popup_22b351ff169e1202a6c9e88864d5523c = L.popup({
  "maxWidth": 350,
});

        
            
                var html_19c9801ee66e2a99a478f68d827869a8 = $(`<div id="html_19c9801ee66e2a99a478f68d827869a8" style="width: 100.0%; height: 100.0%;">         <b style='font-size:12px'>Khu đô thị Vinhomes Riverside</b><br>         <hr style='margin:3px 0'>         <b>❌ NOT SELECTED</b><br>         ID: Site_59<br>         District: D_04<br>         <br>         <b>🏗️ Infrastructure:</b><br>         • Area: 70 m²<br>         • Grid Power: 1000 kW<br>         • Base Load: 650 kW<br>         • Base Cost: 150,000,000 VND         </div>`)[0];
                popup_22b351ff169e1202a6c9e88864d5523c.setContent(html_19c9801ee66e2a99a478f68d827869a8);
            
        

        marker_37a9e816cbe54ad4458f989295bb4a4d.bindPopup(popup_22b351ff169e1202a6c9e88864d5523c)
        ;

        
    
    
            marker_37a9e816cbe54ad4458f989295bb4a4d.bindTooltip(
                `<div>
                     Khu đô thị Vinhomes Riverside (❌ NOT SELECTED)
                 </div>`,
                {
  "sticky": true,
}
            );
        
    
                marker_37a9e816cbe54ad4458f989295bb4a4d.setIcon(icon_44b27971918149696bb29828de1519e6);
            
    
            var marker_80b52283ba24af338208ac1649e28d49 = L.marker(
                [21.0505406825481, 105.893541813492],
                {
}
            ).addTo(map_c8ff09de98adc905a54fc2040c1d5971);
        
    
            var icon_076db85b550048fb937fde4fc9946b93 = L.AwesomeMarkers.icon(
                {
  "markerColor": "red",
  "iconColor": "white",
  "icon": "times",
  "prefix": "fa",
  "extraClasses": "fa-rotate-0",
}
            );
        
    
        var popup_fdddcb322b2ac24e213186710bcb1bf2 = L.popup({
  "maxWidth": 350,
});

        
            
                var html_98526a0004701646e1e8775e9fc3f612 = $(`<div id="html_98526a0004701646e1e8775e9fc3f612" style="width: 100.0%; height: 100.0%;">         <b style='font-size:12px'>Savico MegaMall Long Biên</b><br>         <hr style='margin:3px 0'>         <b>❌ NOT SELECTED</b><br>         ID: Site_60<br>         District: D_04<br>         <br>         <b>🏗️ Infrastructure:</b><br>         • Area: 70 m²<br>         • Grid Power: 1200 kW<br>         • Base Load: 950 kW<br>         • Base Cost: 280,000,000 VND         </div>`)[0];
                popup_fdddcb322b2ac24e213186710bcb1bf2.setContent(html_98526a0004701646e1e8775e9fc3f612);
            
        

        marker_80b52283ba24af338208ac1649e28d49.bindPopup(popup_fdddcb322b2ac24e213186710bcb1bf2)
        ;

        
    
    
            marker_80b52283ba24af338208ac1649e28d49.bindTooltip(
                `<div>
                     Savico MegaMall Long Biên (❌ NOT SELECTED)
                 </div>`,
                {
  "sticky": true,
}
            );
        
    
                marker_80b52283ba24af338208ac1649e28d49.setIcon(icon_076db85b550048fb937fde4fc9946b93);
            
    
            var marker_a3a304dfcb376c3afc464ed1b31677fc = L.marker(
                [21.0461134153963, 105.866600542328],
                {
}
            ).addTo(map_c8ff09de98adc905a54fc2040c1d5971);
        
    
            var icon_fe3c3f1442d2f2e90157a82e333e00fa = L.AwesomeMarkers.icon(
                {
  "markerColor": "red",
  "iconColor": "white",
  "icon": "times",
  "prefix": "fa",
  "extraClasses": "fa-rotate-0",
}
            );
        
    
        var popup_90be3856bce6f584f8585e5dbaf0f189 = L.popup({
  "maxWidth": 350,
});

        
            
                var html_eea3a586d53216bedf99245f69be905e = $(`<div id="html_eea3a586d53216bedf99245f69be905e" style="width: 100.0%; height: 100.0%;">         <b style='font-size:12px'>Chung cư Mipec Riverside</b><br>         <hr style='margin:3px 0'>         <b>❌ NOT SELECTED</b><br>         ID: Site_61<br>         District: D_04<br>         <br>         <b>🏗️ Infrastructure:</b><br>         • Area: 80 m²<br>         • Grid Power: 800 kW<br>         • Base Load: 550 kW<br>         • Base Cost: 200,000,000 VND         </div>`)[0];
                popup_90be3856bce6f584f8585e5dbaf0f189.setContent(html_eea3a586d53216bedf99245f69be905e);
            
        

        marker_a3a304dfcb376c3afc464ed1b31677fc.bindPopup(popup_90be3856bce6f584f8585e5dbaf0f189)
        ;

        
    
    
            marker_a3a304dfcb376c3afc464ed1b31677fc.bindTooltip(
                `<div>
                     Chung cư Mipec Riverside (❌ NOT SELECTED)
                 </div>`,
                {
  "sticky": true,
}
            );
        
    
                marker_a3a304dfcb376c3afc464ed1b31677fc.setIcon(icon_fe3c3f1442d2f2e90157a82e333e00fa);
            
    
            var marker_ee81207fe12c33b1ffbae49b5f76bbf6 = L.marker(
                [21.02170366956, 105.89500131164],
                {
}
            ).addTo(map_c8ff09de98adc905a54fc2040c1d5971);
        
    
            var icon_6e58629d83dab2366f208a31e5e76f47 = L.AwesomeMarkers.icon(
                {
  "markerColor": "green",
  "iconColor": "white",
  "icon": "bolt",
  "prefix": "fa",
  "extraClasses": "fa-rotate-0",
}
            );
        
    
        var popup_fcd565894c1ed0e9cacbba96829633c0 = L.popup({
  "maxWidth": 350,
});

        
            
                var html_55abf5d194879225eeb2861e86630b9e = $(`<div id="html_55abf5d194879225eeb2861e86630b9e" style="width: 100.0%; height: 100.0%;">         <b style='font-size:12px'>Bãi xe Cầu Vĩnh Tuy</b><br>         <hr style='margin:3px 0'>         <b>✅ SELECTED</b><br>         ID: Site_62<br>         District: D_04<br>         <br>         <b>📊 Specifications:</b><br>         • Chargers: <b>9</b> ports<br>         • Power: <b>1350</b> kW<br>         • Output: <b>7,680</b> kWh/day<br>         • Capital: <b>5,520,000,000</b> Million VND<br>         <br>         <b>🏗️ Infrastructure:</b><br>         • Area: 100 m²<br>         • Grid Power: 600 kW<br>         • Base Load: 250 kW         </div>`)[0];
                popup_fcd565894c1ed0e9cacbba96829633c0.setContent(html_55abf5d194879225eeb2861e86630b9e);
            
        

        marker_ee81207fe12c33b1ffbae49b5f76bbf6.bindPopup(popup_fcd565894c1ed0e9cacbba96829633c0)
        ;

        
    
    
            marker_ee81207fe12c33b1ffbae49b5f76bbf6.bindTooltip(
                `<div>
                     Bãi xe Cầu Vĩnh Tuy (✅ SELECTED)
                 </div>`,
                {
  "sticky": true,
}
            );
        
    
                marker_ee81207fe12c33b1ffbae49b5f76bbf6.setIcon(icon_6e58629d83dab2366f208a31e5e76f47);
            
    
            var marker_4fa223fd0f691b4b122c33c4aa0ec047 = L.marker(
                [20.9948298145081, 105.760771770592],
                {
}
            ).addTo(map_c8ff09de98adc905a54fc2040c1d5971);
        
    
            var icon_7a73e2d7c4eb76a18cd56995d68133cc = L.AwesomeMarkers.icon(
                {
  "markerColor": "red",
  "iconColor": "white",
  "icon": "times",
  "prefix": "fa",
  "extraClasses": "fa-rotate-0",
}
            );
        
    
        var popup_7fd630940d5cceef462a7133a3fe1343 = L.popup({
  "maxWidth": 350,
});

        
            
                var html_35b6c85868da220c6a0ebdab9760d7f5 = $(`<div id="html_35b6c85868da220c6a0ebdab9760d7f5" style="width: 100.0%; height: 100.0%;">         <b style='font-size:12px'>Vincom Mega Mall Hà Đông</b><br>         <hr style='margin:3px 0'>         <b>❌ NOT SELECTED</b><br>         ID: Site_63<br>         District: D_12<br>         <br>         <b>🏗️ Infrastructure:</b><br>         • Area: 120 m²<br>         • Grid Power: 1200 kW<br>         • Base Load: 900 kW<br>         • Base Cost: 150,000,000 VND         </div>`)[0];
                popup_7fd630940d5cceef462a7133a3fe1343.setContent(html_35b6c85868da220c6a0ebdab9760d7f5);
            
        

        marker_4fa223fd0f691b4b122c33c4aa0ec047.bindPopup(popup_7fd630940d5cceef462a7133a3fe1343)
        ;

        
    
    
            marker_4fa223fd0f691b4b122c33c4aa0ec047.bindTooltip(
                `<div>
                     Vincom Mega Mall Hà Đông (❌ NOT SELECTED)
                 </div>`,
                {
  "sticky": true,
}
            );
        
    
                marker_4fa223fd0f691b4b122c33c4aa0ec047.setIcon(icon_7a73e2d7c4eb76a18cd56995d68133cc);
            
    
            var marker_972ecab2d5cf5031f6b09ad532b34835 = L.marker(
                [20.989964139743, 105.751727628835],
                {
}
            ).addTo(map_c8ff09de98adc905a54fc2040c1d5971);
        
    
            var icon_8a63ed2bb38d1f03ed32459b7c55b21a = L.AwesomeMarkers.icon(
                {
  "markerColor": "red",
  "iconColor": "white",
  "icon": "times",
  "prefix": "fa",
  "extraClasses": "fa-rotate-0",
}
            );
        
    
        var popup_3f39f9e3baa84da683e354a76608173a = L.popup({
  "maxWidth": 350,
});

        
            
                var html_df183b0eb8cd7934bfdb0ce2c9b5e08d = $(`<div id="html_df183b0eb8cd7934bfdb0ce2c9b5e08d" style="width: 100.0%; height: 100.0%;">         <b style='font-size:12px'>AEON Mall Hà Đông</b><br>         <hr style='margin:3px 0'>         <b>❌ NOT SELECTED</b><br>         ID: Site_64<br>         District: D_12<br>         <br>         <b>🏗️ Infrastructure:</b><br>         • Area: 100 m²<br>         • Grid Power: 1400 kW<br>         • Base Load: 1100 kW<br>         • Base Cost: 150,000,000 VND         </div>`)[0];
                popup_3f39f9e3baa84da683e354a76608173a.setContent(html_df183b0eb8cd7934bfdb0ce2c9b5e08d);
            
        

        marker_972ecab2d5cf5031f6b09ad532b34835.bindPopup(popup_3f39f9e3baa84da683e354a76608173a)
        ;

        
    
    
            marker_972ecab2d5cf5031f6b09ad532b34835.bindTooltip(
                `<div>
                     AEON Mall Hà Đông (❌ NOT SELECTED)
                 </div>`,
                {
  "sticky": true,
}
            );
        
    
                marker_972ecab2d5cf5031f6b09ad532b34835.setIcon(icon_8a63ed2bb38d1f03ed32459b7c55b21a);
            
    
            var marker_f8bdb4bcf77e304c69bc1ae87ce2b28d = L.marker(
                [20.9498094312606, 105.747638484658],
                {
}
            ).addTo(map_c8ff09de98adc905a54fc2040c1d5971);
        
    
            var icon_83085ce02c34423f7e2a81a8e4a35785 = L.AwesomeMarkers.icon(
                {
  "markerColor": "red",
  "iconColor": "white",
  "icon": "times",
  "prefix": "fa",
  "extraClasses": "fa-rotate-0",
}
            );
        
    
        var popup_e93faeab867170563af51a1818f69650 = L.popup({
  "maxWidth": 350,
});

        
            
                var html_6fa356190c9ba93e27fbb8c02c91d5ed = $(`<div id="html_6fa356190c9ba93e27fbb8c02c91d5ed" style="width: 100.0%; height: 100.0%;">         <b style='font-size:12px'>Bến xe Yên Nghĩa</b><br>         <hr style='margin:3px 0'>         <b>❌ NOT SELECTED</b><br>         ID: Site_65<br>         District: D_12<br>         <br>         <b>🏗️ Infrastructure:</b><br>         • Area: 90 m²<br>         • Grid Power: 1500 kW<br>         • Base Load: 1200 kW<br>         • Base Cost: 90,000,000 VND         </div>`)[0];
                popup_e93faeab867170563af51a1818f69650.setContent(html_6fa356190c9ba93e27fbb8c02c91d5ed);
            
        

        marker_f8bdb4bcf77e304c69bc1ae87ce2b28d.bindPopup(popup_e93faeab867170563af51a1818f69650)
        ;

        
    
    
            marker_f8bdb4bcf77e304c69bc1ae87ce2b28d.bindTooltip(
                `<div>
                     Bến xe Yên Nghĩa (❌ NOT SELECTED)
                 </div>`,
                {
  "sticky": true,
}
            );
        
    
                marker_f8bdb4bcf77e304c69bc1ae87ce2b28d.setIcon(icon_83085ce02c34423f7e2a81a8e4a35785);
            
    
            var marker_68377d78b2f8030063487a22217262d3 = L.marker(
                [20.9589179558431, 105.768850671164],
                {
}
            ).addTo(map_c8ff09de98adc905a54fc2040c1d5971);
        
    
            var icon_0ccfa41473ba50569d31a133ab3c291e = L.AwesomeMarkers.icon(
                {
  "markerColor": "red",
  "iconColor": "white",
  "icon": "times",
  "prefix": "fa",
  "extraClasses": "fa-rotate-0",
}
            );
        
    
        var popup_b5da1633a61a167f4b04638beecccb39 = L.popup({
  "maxWidth": 350,
});

        
            
                var html_602daf40ed8e56c73d58c2c552b168a5 = $(`<div id="html_602daf40ed8e56c73d58c2c552b168a5" style="width: 100.0%; height: 100.0%;">         <b style='font-size:12px'>Khu đô thị Văn Phú</b><br>         <hr style='margin:3px 0'>         <b>❌ NOT SELECTED</b><br>         ID: Site_66<br>         District: D_12<br>         <br>         <b>🏗️ Infrastructure:</b><br>         • Area: 80 m²<br>         • Grid Power: 1000 kW<br>         • Base Load: 650 kW<br>         • Base Cost: 100,000,000 VND         </div>`)[0];
                popup_b5da1633a61a167f4b04638beecccb39.setContent(html_602daf40ed8e56c73d58c2c552b168a5);
            
        

        marker_68377d78b2f8030063487a22217262d3.bindPopup(popup_b5da1633a61a167f4b04638beecccb39)
        ;

        
    
    
            marker_68377d78b2f8030063487a22217262d3.bindTooltip(
                `<div>
                     Khu đô thị Văn Phú (❌ NOT SELECTED)
                 </div>`,
                {
  "sticky": true,
}
            );
        
    
                marker_68377d78b2f8030063487a22217262d3.setIcon(icon_0ccfa41473ba50569d31a133ab3c291e);
            
    
            var marker_35b1baf669cb5a32c092567b9699ad15 = L.marker(
                [20.972698557349, 105.758526637798],
                {
}
            ).addTo(map_c8ff09de98adc905a54fc2040c1d5971);
        
    
            var icon_2a0f0a57a85f7c68bf866141be463574 = L.AwesomeMarkers.icon(
                {
  "markerColor": "red",
  "iconColor": "white",
  "icon": "times",
  "prefix": "fa",
  "extraClasses": "fa-rotate-0",
}
            );
        
    
        var popup_968fd8eefd7574357539d447cfb8e0fd = L.popup({
  "maxWidth": 350,
});

        
            
                var html_1c01d8cc495ec6db910e73f4b9f39238 = $(`<div id="html_1c01d8cc495ec6db910e73f4b9f39238" style="width: 100.0%; height: 100.0%;">         <b style='font-size:12px'>Chung cư The Pride</b><br>         <hr style='margin:3px 0'>         <b>❌ NOT SELECTED</b><br>         ID: Site_67<br>         District: D_12<br>         <br>         <b>🏗️ Infrastructure:</b><br>         • Area: 70 m²<br>         • Grid Power: 800 kW<br>         • Base Load: 550 kW<br>         • Base Cost: 80,000,000 VND         </div>`)[0];
                popup_968fd8eefd7574357539d447cfb8e0fd.setContent(html_1c01d8cc495ec6db910e73f4b9f39238);
            
        

        marker_35b1baf669cb5a32c092567b9699ad15.bindPopup(popup_968fd8eefd7574357539d447cfb8e0fd)
        ;

        
    
    
            marker_35b1baf669cb5a32c092567b9699ad15.bindTooltip(
                `<div>
                     Chung cư The Pride (❌ NOT SELECTED)
                 </div>`,
                {
  "sticky": true,
}
            );
        
    
                marker_35b1baf669cb5a32c092567b9699ad15.setIcon(icon_2a0f0a57a85f7c68bf866141be463574);
            
    
            var marker_2006d49cbef7b9eec684a9b222550d7b = L.marker(
                [20.9632401863197, 105.746182928835],
                {
}
            ).addTo(map_c8ff09de98adc905a54fc2040c1d5971);
        
    
            var icon_d631429be6e03f682419616c192b37f6 = L.AwesomeMarkers.icon(
                {
  "markerColor": "green",
  "iconColor": "white",
  "icon": "bolt",
  "prefix": "fa",
  "extraClasses": "fa-rotate-0",
}
            );
        
    
        var popup_42f31d81748b09621d19e362bc11e947 = L.popup({
  "maxWidth": 350,
});

        
            
                var html_5a10dde975a85d151eefc69295c2e5bd = $(`<div id="html_5a10dde975a85d151eefc69295c2e5bd" style="width: 100.0%; height: 100.0%;">         <b style='font-size:12px'>Khu đô thị Dương Nội</b><br>         <hr style='margin:3px 0'>         <b>✅ SELECTED</b><br>         ID: Site_68<br>         District: D_12<br>         <br>         <b>📊 Specifications:</b><br>         • Chargers: <b>9</b> ports<br>         • Power: <b>1350</b> kW<br>         • Output: <b>7,200</b> kWh/day<br>         • Capital: <b>5,500,000,000</b> Million VND<br>         <br>         <b>🏗️ Infrastructure:</b><br>         • Area: 80 m²<br>         • Grid Power: 1000 kW<br>         • Base Load: 650 kW         </div>`)[0];
                popup_42f31d81748b09621d19e362bc11e947.setContent(html_5a10dde975a85d151eefc69295c2e5bd);
            
        

        marker_2006d49cbef7b9eec684a9b222550d7b.bindPopup(popup_42f31d81748b09621d19e362bc11e947)
        ;

        
    
    
            marker_2006d49cbef7b9eec684a9b222550d7b.bindTooltip(
                `<div>
                     Khu đô thị Dương Nội (✅ SELECTED)
                 </div>`,
                {
  "sticky": true,
}
            );
        
    
                marker_2006d49cbef7b9eec684a9b222550d7b.setIcon(icon_d631429be6e03f682419616c192b37f6);
            
    
            var marker_2f1b99b156b9dc3cd7be1eec10d2eec2 = L.marker(
                [20.9644466096936, 105.771818528835],
                {
}
            ).addTo(map_c8ff09de98adc905a54fc2040c1d5971);
        
    
            var icon_cc9ab042445a62eed1c7884a97620536 = L.AwesomeMarkers.icon(
                {
  "markerColor": "red",
  "iconColor": "white",
  "icon": "times",
  "prefix": "fa",
  "extraClasses": "fa-rotate-0",
}
            );
        
    
        var popup_d66e424d5dc1f19453cf103b82ce2901 = L.popup({
  "maxWidth": 350,
});

        
            
                var html_e4780d60f9a5c034b6707b9627ebba38 = $(`<div id="html_e4780d60f9a5c034b6707b9627ebba38" style="width: 100.0%; height: 100.0%;">         <b style='font-size:12px'>Bãi xe Mê Linh Plaza Hà Đông</b><br>         <hr style='margin:3px 0'>         <b>❌ NOT SELECTED</b><br>         ID: Site_69<br>         District: D_12<br>         <br>         <b>🏗️ Infrastructure:</b><br>         • Area: 80 m²<br>         • Grid Power: 600 kW<br>         • Base Load: 250 kW<br>         • Base Cost: 120,000,000 VND         </div>`)[0];
                popup_d66e424d5dc1f19453cf103b82ce2901.setContent(html_e4780d60f9a5c034b6707b9627ebba38);
            
        

        marker_2f1b99b156b9dc3cd7be1eec10d2eec2.bindPopup(popup_d66e424d5dc1f19453cf103b82ce2901)
        ;

        
    
    
            marker_2f1b99b156b9dc3cd7be1eec10d2eec2.bindTooltip(
                `<div>
                     Bãi xe Mê Linh Plaza Hà Đông (❌ NOT SELECTED)
                 </div>`,
                {
  "sticky": true,
}
            );
        
    
                marker_2f1b99b156b9dc3cd7be1eec10d2eec2.setIcon(icon_cc9ab042445a62eed1c7884a97620536);
            
    
            var marker_edecf5ed21156bd7b6e3e04ab96bb1e7 = L.marker(
                [21.0762514334647, 105.812704915341],
                {
}
            ).addTo(map_c8ff09de98adc905a54fc2040c1d5971);
        
    
            var icon_97ed0db7e862c1649a88178eb0c19b0c = L.AwesomeMarkers.icon(
                {
  "markerColor": "red",
  "iconColor": "white",
  "icon": "times",
  "prefix": "fa",
  "extraClasses": "fa-rotate-0",
}
            );
        
    
        var popup_5ecda8cafe72360afb22d58792ebe0e1 = L.popup({
  "maxWidth": 350,
});

        
            
                var html_15fd8af34e6ed0d2c9d2ed88feabe385 = $(`<div id="html_15fd8af34e6ed0d2c9d2ed88feabe385" style="width: 100.0%; height: 100.0%;">         <b style='font-size:12px'>Lotte Mall West Lake Hanoi</b><br>         <hr style='margin:3px 0'>         <b>❌ NOT SELECTED</b><br>         ID: Site_70<br>         District: D_03<br>         <br>         <b>🏗️ Infrastructure:</b><br>         • Area: 90 m²<br>         • Grid Power: 1500 kW<br>         • Base Load: 1200 kW<br>         • Base Cost: 350,000,000 VND         </div>`)[0];
                popup_5ecda8cafe72360afb22d58792ebe0e1.setContent(html_15fd8af34e6ed0d2c9d2ed88feabe385);
            
        

        marker_edecf5ed21156bd7b6e3e04ab96bb1e7.bindPopup(popup_5ecda8cafe72360afb22d58792ebe0e1)
        ;

        
    
    
            marker_edecf5ed21156bd7b6e3e04ab96bb1e7.bindTooltip(
                `<div>
                     Lotte Mall West Lake Hanoi (❌ NOT SELECTED)
                 </div>`,
                {
  "sticky": true,
}
            );
        
    
                marker_edecf5ed21156bd7b6e3e04ab96bb1e7.setIcon(icon_97ed0db7e862c1649a88178eb0c19b0c);
            
    
            var marker_fe9f7d01595836dabfe5852f06f58873 = L.marker(
                [21.0759930025875, 105.809941638091],
                {
}
            ).addTo(map_c8ff09de98adc905a54fc2040c1d5971);
        
    
            var icon_9bd793c1cabf4394dee9f4e972999b90 = L.AwesomeMarkers.icon(
                {
  "markerColor": "green",
  "iconColor": "white",
  "icon": "bolt",
  "prefix": "fa",
  "extraClasses": "fa-rotate-0",
}
            );
        
    
        var popup_75b581dd4d9a8364236b2ebadad753e8 = L.popup({
  "maxWidth": 350,
});

        
            
                var html_4a55b1a5830be6ee5df9a0b91a2d4077 = $(`<div id="html_4a55b1a5830be6ee5df9a0b91a2d4077" style="width: 100.0%; height: 100.0%;">         <b style='font-size:12px'>Ciputra Parking Complex</b><br>         <hr style='margin:3px 0'>         <b>✅ SELECTED</b><br>         ID: Site_71<br>         District: D_03<br>         <br>         <b>📊 Specifications:</b><br>         • Chargers: <b>8</b> ports<br>         • Power: <b>1200</b> kW<br>         • Output: <b>6,960</b> kWh/day<br>         • Capital: <b>5,050,000,000</b> Million VND<br>         <br>         <b>🏗️ Infrastructure:</b><br>         • Area: 90 m²<br>         • Grid Power: 600 kW<br>         • Base Load: 250 kW         </div>`)[0];
                popup_75b581dd4d9a8364236b2ebadad753e8.setContent(html_4a55b1a5830be6ee5df9a0b91a2d4077);
            
        

        marker_fe9f7d01595836dabfe5852f06f58873.bindPopup(popup_75b581dd4d9a8364236b2ebadad753e8)
        ;

        
    
    
            marker_fe9f7d01595836dabfe5852f06f58873.bindTooltip(
                `<div>
                     Ciputra Parking Complex (✅ SELECTED)
                 </div>`,
                {
  "sticky": true,
}
            );
        
    
                marker_fe9f7d01595836dabfe5852f06f58873.setIcon(icon_9bd793c1cabf4394dee9f4e972999b90);
            
    
            var marker_34fedc988d54a1fb1ae610661c007dc2 = L.marker(
                [21.0723619413213, 105.809122169316],
                {
}
            ).addTo(map_c8ff09de98adc905a54fc2040c1d5971);
        
    
            var icon_7e11d665dc56962cd509799d493c67a3 = L.AwesomeMarkers.icon(
                {
  "markerColor": "red",
  "iconColor": "white",
  "icon": "times",
  "prefix": "fa",
  "extraClasses": "fa-rotate-0",
}
            );
        
    
        var popup_9d1f4d2281ba4b91af6b82c5249e4e01 = L.popup({
  "maxWidth": 350,
});

        
            
                var html_e4cb3310e8fef64817e69ee2738fbb6f = $(`<div id="html_e4cb3310e8fef64817e69ee2738fbb6f" style="width: 100.0%; height: 100.0%;">         <b style='font-size:12px'>Khu đô thị Ciputra</b><br>         <hr style='margin:3px 0'>         <b>❌ NOT SELECTED</b><br>         ID: Site_72<br>         District: D_03<br>         <br>         <b>🏗️ Infrastructure:</b><br>         • Area: 70 m²<br>         • Grid Power: 1200 kW<br>         • Base Load: 800 kW<br>         • Base Cost: 250,000,000 VND         </div>`)[0];
                popup_9d1f4d2281ba4b91af6b82c5249e4e01.setContent(html_e4cb3310e8fef64817e69ee2738fbb6f);
            
        

        marker_34fedc988d54a1fb1ae610661c007dc2.bindPopup(popup_9d1f4d2281ba4b91af6b82c5249e4e01)
        ;

        
    
    
            marker_34fedc988d54a1fb1ae610661c007dc2.bindTooltip(
                `<div>
                     Khu đô thị Ciputra (❌ NOT SELECTED)
                 </div>`,
                {
  "sticky": true,
}
            );
        
    
                marker_34fedc988d54a1fb1ae610661c007dc2.setIcon(icon_7e11d665dc56962cd509799d493c67a3);
            
    
            var marker_36126a261aae9eb1b55847a5422a148b = L.marker(
                [21.0731626037496, 105.817198098152],
                {
}
            ).addTo(map_c8ff09de98adc905a54fc2040c1d5971);
        
    
            var icon_9b180d7a045a8c3f8a2ac814a4ce402b = L.AwesomeMarkers.icon(
                {
  "markerColor": "red",
  "iconColor": "white",
  "icon": "times",
  "prefix": "fa",
  "extraClasses": "fa-rotate-0",
}
            );
        
    
        var popup_e97913049ef1f7540afedba4d24d4bec = L.popup({
  "maxWidth": 350,
});

        
            
                var html_f3a3860e25248b2d7b4ca7d5dfc2a7da = $(`<div id="html_f3a3860e25248b2d7b4ca7d5dfc2a7da" style="width: 100.0%; height: 100.0%;">         <b style='font-size:12px'>Công viên nước Hồ Tây</b><br>         <hr style='margin:3px 0'>         <b>❌ NOT SELECTED</b><br>         ID: Site_73<br>         District: D_03<br>         <br>         <b>🏗️ Infrastructure:</b><br>         • Area: 100 m²<br>         • Grid Power: 800 kW<br>         • Base Load: 350 kW<br>         • Base Cost: 200,000,000 VND         </div>`)[0];
                popup_e97913049ef1f7540afedba4d24d4bec.setContent(html_f3a3860e25248b2d7b4ca7d5dfc2a7da);
            
        

        marker_36126a261aae9eb1b55847a5422a148b.bindPopup(popup_e97913049ef1f7540afedba4d24d4bec)
        ;

        
    
    
            marker_36126a261aae9eb1b55847a5422a148b.bindTooltip(
                `<div>
                     Công viên nước Hồ Tây (❌ NOT SELECTED)
                 </div>`,
                {
  "sticky": true,
}
            );
        
    
                marker_36126a261aae9eb1b55847a5422a148b.setIcon(icon_9b180d7a045a8c3f8a2ac814a4ce402b);
            
    
            var marker_f5e5f7df69dbf1aee32bab61e655b166 = L.marker(
                [21.0610906305142, 105.831916684658],
                {
}
            ).addTo(map_c8ff09de98adc905a54fc2040c1d5971);
        
    
            var icon_a1a8a41706ce4de5159fa120186079b9 = L.AwesomeMarkers.icon(
                {
  "markerColor": "red",
  "iconColor": "white",
  "icon": "times",
  "prefix": "fa",
  "extraClasses": "fa-rotate-0",
}
            );
        
    
        var popup_89e01fa8a3de5e8319d99cfff53740fd = L.popup({
  "maxWidth": 350,
});

        
            
                var html_3216f17f3bb185272c035a604097f902 = $(`<div id="html_3216f17f3bb185272c035a604097f902" style="width: 100.0%; height: 100.0%;">         <b style='font-size:12px'>Sheraton Hanoi Hotel Parking</b><br>         <hr style='margin:3px 0'>         <b>❌ NOT SELECTED</b><br>         ID: Site_74<br>         District: D_03<br>         <br>         <b>🏗️ Infrastructure:</b><br>         • Area: 80 m²<br>         • Grid Power: 1000 kW<br>         • Base Load: 750 kW<br>         • Base Cost: 300,000,000 VND         </div>`)[0];
                popup_89e01fa8a3de5e8319d99cfff53740fd.setContent(html_3216f17f3bb185272c035a604097f902);
            
        

        marker_f5e5f7df69dbf1aee32bab61e655b166.bindPopup(popup_89e01fa8a3de5e8319d99cfff53740fd)
        ;

        
    
    
            marker_f5e5f7df69dbf1aee32bab61e655b166.bindTooltip(
                `<div>
                     Sheraton Hanoi Hotel Parking (❌ NOT SELECTED)
                 </div>`,
                {
  "sticky": true,
}
            );
        
    
                marker_f5e5f7df69dbf1aee32bab61e655b166.setIcon(icon_a1a8a41706ce4de5159fa120186079b9);
            
    
            var marker_5e6a671374464638c603f1562926bf4f = L.marker(
                [21.0521750056121, 105.808481528835],
                {
}
            ).addTo(map_c8ff09de98adc905a54fc2040c1d5971);
        
    
            var icon_26c18767f238c9693b636274491ace6b = L.AwesomeMarkers.icon(
                {
  "markerColor": "red",
  "iconColor": "white",
  "icon": "times",
  "prefix": "fa",
  "extraClasses": "fa-rotate-0",
}
            );
        
    
        var popup_a717046e0df404190e2309a78ff11fc8 = L.popup({
  "maxWidth": 350,
});

        
            
                var html_02ee7ea8a1f401b2956457a9fad5a5e6 = $(`<div id="html_02ee7ea8a1f401b2956457a9fad5a5e6" style="width: 100.0%; height: 100.0%;">         <b style='font-size:12px'>Chung cư Watermark Hồ Tây</b><br>         <hr style='margin:3px 0'>         <b>❌ NOT SELECTED</b><br>         ID: Site_75<br>         District: D_03<br>         <br>         <b>🏗️ Infrastructure:</b><br>         • Area: 70 m²<br>         • Grid Power: 900 kW<br>         • Base Load: 650 kW<br>         • Base Cost: 220,000,000 VND         </div>`)[0];
                popup_a717046e0df404190e2309a78ff11fc8.setContent(html_02ee7ea8a1f401b2956457a9fad5a5e6);
            
        

        marker_5e6a671374464638c603f1562926bf4f.bindPopup(popup_a717046e0df404190e2309a78ff11fc8)
        ;

        
    
    
            marker_5e6a671374464638c603f1562926bf4f.bindTooltip(
                `<div>
                     Chung cư Watermark Hồ Tây (❌ NOT SELECTED)
                 </div>`,
                {
  "sticky": true,
}
            );
        
    
                marker_5e6a671374464638c603f1562926bf4f.setIcon(icon_26c18767f238c9693b636274491ace6b);
            
    
            var marker_b6090a01162ad3b1c61e5dc8710f32e8 = L.marker(
                [21.0553615255241, 105.819707342329],
                {
}
            ).addTo(map_c8ff09de98adc905a54fc2040c1d5971);
        
    
            var icon_cad434cec9f23721e65896ad9e26132e = L.AwesomeMarkers.icon(
                {
  "markerColor": "red",
  "iconColor": "white",
  "icon": "times",
  "prefix": "fa",
  "extraClasses": "fa-rotate-0",
}
            );
        
    
        var popup_c2a3168871ce6cb51c8de11b274dd713 = L.popup({
  "maxWidth": 350,
});

        
            
                var html_35a64d70e4a3208db05e95604a8a490b = $(`<div id="html_35a64d70e4a3208db05e95604a8a490b" style="width: 100.0%; height: 100.0%;">         <b style='font-size:12px'>Bãi đỗ xe Phủ Tây Hồ</b><br>         <hr style='margin:3px 0'>         <b>❌ NOT SELECTED</b><br>         ID: Site_76<br>         District: D_03<br>         <br>         <b>🏗️ Infrastructure:</b><br>         • Area: 90 m²<br>         • Grid Power: 500 kW<br>         • Base Load: 200 kW<br>         • Base Cost: 150,000,000 VND         </div>`)[0];
                popup_c2a3168871ce6cb51c8de11b274dd713.setContent(html_35a64d70e4a3208db05e95604a8a490b);
            
        

        marker_b6090a01162ad3b1c61e5dc8710f32e8.bindPopup(popup_c2a3168871ce6cb51c8de11b274dd713)
        ;

        
    
    
            marker_b6090a01162ad3b1c61e5dc8710f32e8.bindTooltip(
                `<div>
                     Bãi đỗ xe Phủ Tây Hồ (❌ NOT SELECTED)
                 </div>`,
                {
  "sticky": true,
}
            );
        
    
                marker_b6090a01162ad3b1c61e5dc8710f32e8.setIcon(icon_cad434cec9f23721e65896ad9e26132e);
            
    
            var marker_1dc43eab709063b970ccb25f27aa8a61 = L.marker(
                [21.0723305958316, 105.774014830683],
                {
}
            ).addTo(map_c8ff09de98adc905a54fc2040c1d5971);
        
    
            var icon_d3d85b21bf5d48c72bb835089ab921a7 = L.AwesomeMarkers.icon(
                {
  "markerColor": "green",
  "iconColor": "white",
  "icon": "bolt",
  "prefix": "fa",
  "extraClasses": "fa-rotate-0",
}
            );
        
    
        var popup_6a1c14dc43183115f712c1ed6491b795 = L.popup({
  "maxWidth": 350,
});

        
            
                var html_390650b53e001b628c23f32eec26f29a = $(`<div id="html_390650b53e001b628c23f32eec26f29a" style="width: 100.0%; height: 100.0%;">         <b style='font-size:12px'>Đại học Mỏ Địa Chất Parking</b><br>         <hr style='margin:3px 0'>         <b>✅ SELECTED</b><br>         ID: Site_77<br>         District: D_10<br>         <br>         <b>📊 Specifications:</b><br>         • Chargers: <b>8</b> ports<br>         • Power: <b>1200</b> kW<br>         • Output: <b>6,480</b> kWh/day<br>         • Capital: <b>4,920,000,000</b> Million VND<br>         <br>         <b>🏗️ Infrastructure:</b><br>         • Area: 100 m²<br>         • Grid Power: 600 kW<br>         • Base Load: 300 kW         </div>`)[0];
                popup_6a1c14dc43183115f712c1ed6491b795.setContent(html_390650b53e001b628c23f32eec26f29a);
            
        

        marker_1dc43eab709063b970ccb25f27aa8a61.bindPopup(popup_6a1c14dc43183115f712c1ed6491b795)
        ;

        
    
    
            marker_1dc43eab709063b970ccb25f27aa8a61.bindTooltip(
                `<div>
                     Đại học Mỏ Địa Chất Parking (✅ SELECTED)
                 </div>`,
                {
  "sticky": true,
}
            );
        
    
                marker_1dc43eab709063b970ccb25f27aa8a61.setIcon(icon_d3d85b21bf5d48c72bb835089ab921a7);
            
    
            var marker_8b843c7b7882ae31e15d0cc0ab9a8e92 = L.marker(
                [21.0642191980952, 105.787621915341],
                {
}
            ).addTo(map_c8ff09de98adc905a54fc2040c1d5971);
        
    
            var icon_d4df04fe19e5898d5a6deb910924989c = L.AwesomeMarkers.icon(
                {
  "markerColor": "red",
  "iconColor": "white",
  "icon": "times",
  "prefix": "fa",
  "extraClasses": "fa-rotate-0",
}
            );
        
    
        var popup_d50318bd834a34f6624faabb50212a9b = L.popup({
  "maxWidth": 350,
});

        
            
                var html_d7e78e6ada6c8543aecbe7a8fc19f409 = $(`<div id="html_d7e78e6ada6c8543aecbe7a8fc19f409" style="width: 100.0%; height: 100.0%;">         <b style='font-size:12px'>Công viên Hòa Bình</b><br>         <hr style='margin:3px 0'>         <b>❌ NOT SELECTED</b><br>         ID: Site_78<br>         District: D_10<br>         <br>         <b>🏗️ Infrastructure:</b><br>         • Area: 100 m²<br>         • Grid Power: 800 kW<br>         • Base Load: 350 kW<br>         • Base Cost: 150,000,000 VND         </div>`)[0];
                popup_d50318bd834a34f6624faabb50212a9b.setContent(html_d7e78e6ada6c8543aecbe7a8fc19f409);
            
        

        marker_8b843c7b7882ae31e15d0cc0ab9a8e92.bindPopup(popup_d50318bd834a34f6624faabb50212a9b)
        ;

        
    
    
            marker_8b843c7b7882ae31e15d0cc0ab9a8e92.bindTooltip(
                `<div>
                     Công viên Hòa Bình (❌ NOT SELECTED)
                 </div>`,
                {
  "sticky": true,
}
            );
        
    
                marker_8b843c7b7882ae31e15d0cc0ab9a8e92.setIcon(icon_d4df04fe19e5898d5a6deb910924989c);
            
    
            var marker_cfa12262e38d5a4b670f38162aae5c14 = L.marker(
                [21.0696987120028, 105.797519099999],
                {
}
            ).addTo(map_c8ff09de98adc905a54fc2040c1d5971);
        
    
            var icon_f78195e4e5acc8e39a9cd1bb67b53f05 = L.AwesomeMarkers.icon(
                {
  "markerColor": "red",
  "iconColor": "white",
  "icon": "times",
  "prefix": "fa",
  "extraClasses": "fa-rotate-0",
}
            );
        
    
        var popup_c8fde3dcf2160e9f5ed2ee9b066663b8 = L.popup({
  "maxWidth": 350,
});

        
            
                var html_c02ed69764d5ccfc1770859baf2a7838 = $(`<div id="html_c02ed69764d5ccfc1770859baf2a7838" style="width: 100.0%; height: 100.0%;">         <b style='font-size:12px'>Khu đô thị Ngoại Giao Đoàn</b><br>         <hr style='margin:3px 0'>         <b>❌ NOT SELECTED</b><br>         ID: Site_79<br>         District: D_10<br>         <br>         <b>🏗️ Infrastructure:</b><br>         • Area: 90 m²<br>         • Grid Power: 1200 kW<br>         • Base Load: 800 kW<br>         • Base Cost: 200,000,000 VND         </div>`)[0];
                popup_c8fde3dcf2160e9f5ed2ee9b066663b8.setContent(html_c02ed69764d5ccfc1770859baf2a7838);
            
        

        marker_cfa12262e38d5a4b670f38162aae5c14.bindPopup(popup_c8fde3dcf2160e9f5ed2ee9b066663b8)
        ;

        
    
    
            marker_cfa12262e38d5a4b670f38162aae5c14.bindTooltip(
                `<div>
                     Khu đô thị Ngoại Giao Đoàn (❌ NOT SELECTED)
                 </div>`,
                {
  "sticky": true,
}
            );
        
    
                marker_cfa12262e38d5a4b670f38162aae5c14.setIcon(icon_f78195e4e5acc8e39a9cd1bb67b53f05);
            
    
            var marker_337b69dda4af2166ce6c1aec5fed529c = L.marker(
                [21.053246216553, 105.7800935],
                {
}
            ).addTo(map_c8ff09de98adc905a54fc2040c1d5971);
        
    
            var icon_bf6bce2f5d9c98c515b0f1c387e288e0 = L.AwesomeMarkers.icon(
                {
  "markerColor": "green",
  "iconColor": "white",
  "icon": "bolt",
  "prefix": "fa",
  "extraClasses": "fa-rotate-0",
}
            );
        
    
        var popup_a93dd5f7ea8d60dfb86958ccf1279b3a = L.popup({
  "maxWidth": 350,
});

        
            
                var html_fa29f5c0794f200bff740d943e9add8f = $(`<div id="html_fa29f5c0794f200bff740d943e9add8f" style="width: 100.0%; height: 100.0%;">         <b style='font-size:12px'>Chung cư Green Stars</b><br>         <hr style='margin:3px 0'>         <b>✅ SELECTED</b><br>         ID: Site_80<br>         District: D_10<br>         <br>         <b>📊 Specifications:</b><br>         • Chargers: <b>7</b> ports<br>         • Power: <b>1050</b> kW<br>         • Output: <b>4,920</b> kWh/day<br>         • Capital: <b>4,400,000,000</b> Million VND<br>         <br>         <b>🏗️ Infrastructure:</b><br>         • Area: 70 m²<br>         • Grid Power: 900 kW<br>         • Base Load: 650 kW         </div>`)[0];
                popup_a93dd5f7ea8d60dfb86958ccf1279b3a.setContent(html_fa29f5c0794f200bff740d943e9add8f);
            
        

        marker_337b69dda4af2166ce6c1aec5fed529c.bindPopup(popup_a93dd5f7ea8d60dfb86958ccf1279b3a)
        ;

        
    
    
            marker_337b69dda4af2166ce6c1aec5fed529c.bindTooltip(
                `<div>
                     Chung cư Green Stars (✅ SELECTED)
                 </div>`,
                {
  "sticky": true,
}
            );
        
    
                marker_337b69dda4af2166ce6c1aec5fed529c.setIcon(icon_bf6bce2f5d9c98c515b0f1c387e288e0);
            
    
            var marker_6788e17e1cfd2b794853866f52ed822a = L.marker(
                [21.0396087150024, 105.781930122749],
                {
}
            ).addTo(map_c8ff09de98adc905a54fc2040c1d5971);
        
    
            var icon_861c30eeeb95fdae83148d1b636306f8 = L.AwesomeMarkers.icon(
                {
  "markerColor": "red",
  "iconColor": "white",
  "icon": "times",
  "prefix": "fa",
  "extraClasses": "fa-rotate-0",
}
            );
        
    
        var popup_c76c42f20371b008d6d6bd42f0121813 = L.popup({
  "maxWidth": 350,
});

        
            
                var html_aea6a27b60333c5f8817048a5e5b51c9 = $(`<div id="html_aea6a27b60333c5f8817048a5e5b51c9" style="width: 100.0%; height: 100.0%;">         <b style='font-size:12px'>Bãi đỗ xe Phạm Văn Đồng</b><br>         <hr style='margin:3px 0'>         <b>❌ NOT SELECTED</b><br>         ID: Site_81<br>         District: D_10<br>         <br>         <b>🏗️ Infrastructure:</b><br>         • Area: 80 m²<br>         • Grid Power: 600 kW<br>         • Base Load: 250 kW<br>         • Base Cost: 150,000,000 VND         </div>`)[0];
                popup_c76c42f20371b008d6d6bd42f0121813.setContent(html_aea6a27b60333c5f8817048a5e5b51c9);
            
        

        marker_6788e17e1cfd2b794853866f52ed822a.bindPopup(popup_c76c42f20371b008d6d6bd42f0121813)
        ;

        
    
    
            marker_6788e17e1cfd2b794853866f52ed822a.bindTooltip(
                `<div>
                     Bãi đỗ xe Phạm Văn Đồng (❌ NOT SELECTED)
                 </div>`,
                {
  "sticky": true,
}
            );
        
    
                marker_6788e17e1cfd2b794853866f52ed822a.setIcon(icon_861c30eeeb95fdae83148d1b636306f8);
            
    
            var marker_3a535b0c2787cd5d7fdf80d412f4bd16 = L.marker(
                [21.0545963394432, 105.779075284658],
                {
}
            ).addTo(map_c8ff09de98adc905a54fc2040c1d5971);
        
    
            var icon_055c6f95e2625ed41f137d5287c4e3c4 = L.AwesomeMarkers.icon(
                {
  "markerColor": "red",
  "iconColor": "white",
  "icon": "times",
  "prefix": "fa",
  "extraClasses": "fa-rotate-0",
}
            );
        
    
        var popup_c45bd830d244f1cdfa5e6d8773101dd4 = L.popup({
  "maxWidth": 350,
});

        
            
                var html_895e1c0cdb3b938a08bbee1c000b8ecb = $(`<div id="html_895e1c0cdb3b938a08bbee1c000b8ecb" style="width: 100.0%; height: 100.0%;">         <b style='font-size:12px'>Khu đô thị Thành phố Giao Lưu</b><br>         <hr style='margin:3px 0'>         <b>❌ NOT SELECTED</b><br>         ID: Site_82<br>         District: D_10<br>         <br>         <b>🏗️ Infrastructure:</b><br>         • Area: 80 m²<br>         • Grid Power: 1000 kW<br>         • Base Load: 650 kW<br>         • Base Cost: 200,000,000 VND         </div>`)[0];
                popup_c45bd830d244f1cdfa5e6d8773101dd4.setContent(html_895e1c0cdb3b938a08bbee1c000b8ecb);
            
        

        marker_3a535b0c2787cd5d7fdf80d412f4bd16.bindPopup(popup_c45bd830d244f1cdfa5e6d8773101dd4)
        ;

        
    
    
            marker_3a535b0c2787cd5d7fdf80d412f4bd16.bindTooltip(
                `<div>
                     Khu đô thị Thành phố Giao Lưu (❌ NOT SELECTED)
                 </div>`,
                {
  "sticky": true,
}
            );
        
    
                marker_3a535b0c2787cd5d7fdf80d412f4bd16.setIcon(icon_055c6f95e2625ed41f137d5287c4e3c4);
            
    
            var marker_b2cbf593196a58236bfe392270b5c87e = L.marker(
                [21.0535151723472, 105.775812331529],
                {
}
            ).addTo(map_c8ff09de98adc905a54fc2040c1d5971);
        
    
            var icon_3cf91eba70c4769f9f388968dd06788c = L.AwesomeMarkers.icon(
                {
  "markerColor": "red",
  "iconColor": "white",
  "icon": "times",
  "prefix": "fa",
  "extraClasses": "fa-rotate-0",
}
            );
        
    
        var popup_3ea8cc6ab1d82b270a3b4b961ee8e23a = L.popup({
  "maxWidth": 350,
});

        
            
                var html_55f23109cff0c7cd32341eb3d6876c76 = $(`<div id="html_55f23109cff0c7cd32341eb3d6876c76" style="width: 100.0%; height: 100.0%;">         <b style='font-size:12px'>Bãi xe Bộ Công An Cổ Nhuế</b><br>         <hr style='margin:3px 0'>         <b>❌ NOT SELECTED</b><br>         ID: Site_83<br>         District: D_10<br>         <br>         <b>🏗️ Infrastructure:</b><br>         • Area: 70 m²<br>         • Grid Power: 500 kW<br>         • Base Load: 200 kW<br>         • Base Cost: 120,000,000 VND         </div>`)[0];
                popup_3ea8cc6ab1d82b270a3b4b961ee8e23a.setContent(html_55f23109cff0c7cd32341eb3d6876c76);
            
        

        marker_b2cbf593196a58236bfe392270b5c87e.bindPopup(popup_3ea8cc6ab1d82b270a3b4b961ee8e23a)
        ;

        
    
    
            marker_b2cbf593196a58236bfe392270b5c87e.bindTooltip(
                `<div>
                     Bãi xe Bộ Công An Cổ Nhuế (❌ NOT SELECTED)
                 </div>`,
                {
  "sticky": true,
}
            );
        
    
                marker_b2cbf593196a58236bfe392270b5c87e.setIcon(icon_3cf91eba70c4769f9f388968dd06788c);
            
    
            var marker_0111f9504e523a0cb15ae333ee53c051 = L.marker(
                [21.0154700560823, 105.777696957672],
                {
}
            ).addTo(map_c8ff09de98adc905a54fc2040c1d5971);
        
    
            var icon_e70368ee1aa02912855ec1ec238adc45 = L.AwesomeMarkers.icon(
                {
  "markerColor": "green",
  "iconColor": "white",
  "icon": "bolt",
  "prefix": "fa",
  "extraClasses": "fa-rotate-0",
}
            );
        
    
        var popup_26822069c3fefe4e6011d96f618b1e0f = L.popup({
  "maxWidth": 350,
});

        
            
                var html_5a33fa033c75438395723a376068b874 = $(`<div id="html_5a33fa033c75438395723a376068b874" style="width: 100.0%; height: 100.0%;">         <b style='font-size:12px'>Vincom Plaza The Garden</b><br>         <hr style='margin:3px 0'>         <b>✅ SELECTED</b><br>         ID: Site_84<br>         District: D_11<br>         <br>         <b>📊 Specifications:</b><br>         • Chargers: <b>7</b> ports<br>         • Power: <b>1050</b> kW<br>         • Output: <b>4,800</b> kWh/day<br>         • Capital: <b>4,300,000,000</b> Million VND<br>         <br>         <b>🏗️ Infrastructure:</b><br>         • Area: 60 m²<br>         • Grid Power: 1000 kW<br>         • Base Load: 750 kW         </div>`)[0];
                popup_26822069c3fefe4e6011d96f618b1e0f.setContent(html_5a33fa033c75438395723a376068b874);
            
        

        marker_0111f9504e523a0cb15ae333ee53c051.bindPopup(popup_26822069c3fefe4e6011d96f618b1e0f)
        ;

        
    
    
            marker_0111f9504e523a0cb15ae333ee53c051.bindTooltip(
                `<div>
                     Vincom Plaza The Garden (✅ SELECTED)
                 </div>`,
                {
  "sticky": true,
}
            );
        
    
                marker_0111f9504e523a0cb15ae333ee53c051.setIcon(icon_e70368ee1aa02912855ec1ec238adc45);
            
    
            var marker_6c143d9b2d0681a578cec5d3358d7a47 = L.marker(
                [21.0184959299305, 105.78410135582],
                {
}
            ).addTo(map_c8ff09de98adc905a54fc2040c1d5971);
        
    
            var icon_f9b6dae57e9cc94f446ce6a909c9fa16 = L.AwesomeMarkers.icon(
                {
  "markerColor": "red",
  "iconColor": "white",
  "icon": "times",
  "prefix": "fa",
  "extraClasses": "fa-rotate-0",
}
            );
        
    
        var popup_f23326d726244db24739dbca6f525511 = L.popup({
  "maxWidth": 350,
});

        
            
                var html_2fb59a857f846a0c4bce997bdf6ac989 = $(`<div id="html_2fb59a857f846a0c4bce997bdf6ac989" style="width: 100.0%; height: 100.0%;">         <b style='font-size:12px'>Keangnam Landmark Tower</b><br>         <hr style='margin:3px 0'>         <b>❌ NOT SELECTED</b><br>         ID: Site_85<br>         District: D_11<br>         <br>         <b>🏗️ Infrastructure:</b><br>         • Area: 60 m²<br>         • Grid Power: 1500 kW<br>         • Base Load: 1200 kW<br>         • Base Cost: 200,000,000 VND         </div>`)[0];
                popup_f23326d726244db24739dbca6f525511.setContent(html_2fb59a857f846a0c4bce997bdf6ac989);
            
        

        marker_6c143d9b2d0681a578cec5d3358d7a47.bindPopup(popup_f23326d726244db24739dbca6f525511)
        ;

        
    
    
            marker_6c143d9b2d0681a578cec5d3358d7a47.bindTooltip(
                `<div>
                     Keangnam Landmark Tower (❌ NOT SELECTED)
                 </div>`,
                {
  "sticky": true,
}
            );
        
    
                marker_6c143d9b2d0681a578cec5d3358d7a47.setIcon(icon_f9b6dae57e9cc94f446ce6a909c9fa16);
            
    
            var marker_4036dfc86b8cf480e1a2ac5a0ff2c151 = L.marker(
                [21.0207737453963, 105.765192369312],
                {
}
            ).addTo(map_c8ff09de98adc905a54fc2040c1d5971);
        
    
            var icon_51f7f397bb21e6e3670e6646e70b8398 = L.AwesomeMarkers.icon(
                {
  "markerColor": "red",
  "iconColor": "white",
  "icon": "times",
  "prefix": "fa",
  "extraClasses": "fa-rotate-0",
}
            );
        
    
        var popup_2a3a12d07fe1781181ea576d4d5ae8c8 = L.popup({
  "maxWidth": 350,
});

        
            
                var html_f03166a7a1385a72237ee8bbc44b5f5b = $(`<div id="html_f03166a7a1385a72237ee8bbc44b5f5b" style="width: 100.0%; height: 100.0%;">         <b style='font-size:12px'>Sân vận động Mỹ Đình</b><br>         <hr style='margin:3px 0'>         <b>❌ NOT SELECTED</b><br>         ID: Site_86<br>         District: D_11<br>         <br>         <b>🏗️ Infrastructure:</b><br>         • Area: 100 m²<br>         • Grid Power: 2000 kW<br>         • Base Load: 1600 kW<br>         • Base Cost: 120,000,000 VND         </div>`)[0];
                popup_2a3a12d07fe1781181ea576d4d5ae8c8.setContent(html_f03166a7a1385a72237ee8bbc44b5f5b);
            
        

        marker_4036dfc86b8cf480e1a2ac5a0ff2c151.bindPopup(popup_2a3a12d07fe1781181ea576d4d5ae8c8)
        ;

        
    
    
            marker_4036dfc86b8cf480e1a2ac5a0ff2c151.bindTooltip(
                `<div>
                     Sân vận động Mỹ Đình (❌ NOT SELECTED)
                 </div>`,
                {
  "sticky": true,
}
            );
        
    
                marker_4036dfc86b8cf480e1a2ac5a0ff2c151.setIcon(icon_51f7f397bb21e6e3670e6646e70b8398);
            
    
            var marker_5305a6c366cf3308ce2055fb0717b823 = L.marker(
                [21.0058713961374, 105.787638986507],
                {
}
            ).addTo(map_c8ff09de98adc905a54fc2040c1d5971);
        
    
            var icon_794abe103bfe0c3a0d5ae06e70f20356 = L.AwesomeMarkers.icon(
                {
  "markerColor": "red",
  "iconColor": "white",
  "icon": "times",
  "prefix": "fa",
  "extraClasses": "fa-rotate-0",
}
            );
        
    
        var popup_86badd4efa2f33b83b6d7d9b85e2a2a2 = L.popup({
  "maxWidth": 350,
});

        
            
                var html_6411bc5e5f0e96784c0176597e857a0a = $(`<div id="html_6411bc5e5f0e96784c0176597e857a0a" style="width: 100.0%; height: 100.0%;">         <b style='font-size:12px'>Trung tâm Hội nghị Quốc gia</b><br>         <hr style='margin:3px 0'>         <b>❌ NOT SELECTED</b><br>         ID: Site_87<br>         District: D_11<br>         <br>         <b>🏗️ Infrastructure:</b><br>         • Area: 100 m²<br>         • Grid Power: 1800 kW<br>         • Base Load: 1400 kW<br>         • Base Cost: 200,000,000 VND         </div>`)[0];
                popup_86badd4efa2f33b83b6d7d9b85e2a2a2.setContent(html_6411bc5e5f0e96784c0176597e857a0a);
            
        

        marker_5305a6c366cf3308ce2055fb0717b823.bindPopup(popup_86badd4efa2f33b83b6d7d9b85e2a2a2)
        ;

        
    
    
            marker_5305a6c366cf3308ce2055fb0717b823.bindTooltip(
                `<div>
                     Trung tâm Hội nghị Quốc gia (❌ NOT SELECTED)
                 </div>`,
                {
  "sticky": true,
}
            );
        
    
                marker_5305a6c366cf3308ce2055fb0717b823.setIcon(icon_794abe103bfe0c3a0d5ae06e70f20356);
            
    
            var marker_1474cd1c9ed8151bda8cea4e5c4a4e58 = L.marker(
                [21.0018388200846, 105.782700169258],
                {
}
            ).addTo(map_c8ff09de98adc905a54fc2040c1d5971);
        
    
            var icon_a2fa74d8b2ae3c11de4a0f5426bc73d9 = L.AwesomeMarkers.icon(
                {
  "markerColor": "red",
  "iconColor": "white",
  "icon": "times",
  "prefix": "fa",
  "extraClasses": "fa-rotate-0",
}
            );
        
    
        var popup_cbc675ac216e480f565bc9f3943973b5 = L.popup({
  "maxWidth": 350,
});

        
            
                var html_fce7959e8949b8f8301a75b9fe6a3570 = $(`<div id="html_fce7959e8949b8f8301a75b9fe6a3570" style="width: 100.0%; height: 100.0%;">         <b style='font-size:12px'>Chung cư Vinhomes Green Bay</b><br>         <hr style='margin:3px 0'>         <b>❌ NOT SELECTED</b><br>         ID: Site_88<br>         District: D_11<br>         <br>         <b>🏗️ Infrastructure:</b><br>         • Area: 60 m²<br>         • Grid Power: 1000 kW<br>         • Base Load: 700 kW<br>         • Base Cost: 180,000,000 VND         </div>`)[0];
                popup_cbc675ac216e480f565bc9f3943973b5.setContent(html_fce7959e8949b8f8301a75b9fe6a3570);
            
        

        marker_1474cd1c9ed8151bda8cea4e5c4a4e58.bindPopup(popup_cbc675ac216e480f565bc9f3943973b5)
        ;

        
    
    
            marker_1474cd1c9ed8151bda8cea4e5c4a4e58.bindTooltip(
                `<div>
                     Chung cư Vinhomes Green Bay (❌ NOT SELECTED)
                 </div>`,
                {
  "sticky": true,
}
            );
        
    
                marker_1474cd1c9ed8151bda8cea4e5c4a4e58.setIcon(icon_a2fa74d8b2ae3c11de4a0f5426bc73d9);
            
    
            var marker_5647c956e136169a4359d8a7e9964fb0 = L.marker(
                [21.0286884862292, 105.777203025132],
                {
}
            ).addTo(map_c8ff09de98adc905a54fc2040c1d5971);
        
    
            var icon_af768fdb76048a7c525dab7ba7781f00 = L.AwesomeMarkers.icon(
                {
  "markerColor": "red",
  "iconColor": "white",
  "icon": "times",
  "prefix": "fa",
  "extraClasses": "fa-rotate-0",
}
            );
        
    
        var popup_80b6748bc039f6dffc087aae152f28d4 = L.popup({
  "maxWidth": 350,
});

        
            
                var html_243169ee9f466ff1870c14434263b282 = $(`<div id="html_243169ee9f466ff1870c14434263b282" style="width: 100.0%; height: 100.0%;">         <b style='font-size:12px'>Bến xe Mỹ Đình</b><br>         <hr style='margin:3px 0'>         <b>❌ NOT SELECTED</b><br>         ID: Site_89<br>         District: D_11<br>         <br>         <b>🏗️ Infrastructure:</b><br>         • Area: 100 m²<br>         • Grid Power: 1500 kW<br>         • Base Load: 1200 kW<br>         • Base Cost: 150,000,000 VND         </div>`)[0];
                popup_80b6748bc039f6dffc087aae152f28d4.setContent(html_243169ee9f466ff1870c14434263b282);
            
        

        marker_5647c956e136169a4359d8a7e9964fb0.bindPopup(popup_80b6748bc039f6dffc087aae152f28d4)
        ;

        
    
    
            marker_5647c956e136169a4359d8a7e9964fb0.bindTooltip(
                `<div>
                     Bến xe Mỹ Đình (❌ NOT SELECTED)
                 </div>`,
                {
  "sticky": true,
}
            );
        
    
                marker_5647c956e136169a4359d8a7e9964fb0.setIcon(icon_af768fdb76048a7c525dab7ba7781f00);
            
    
            var marker_bf02b94c217e09a3b4b0fe172672f5c6 = L.marker(
                [21.0147179118105, 105.777807342327],
                {
}
            ).addTo(map_c8ff09de98adc905a54fc2040c1d5971);
        
    
            var icon_4e2cf668b2e2876154b6787b15e25813 = L.AwesomeMarkers.icon(
                {
  "markerColor": "red",
  "iconColor": "white",
  "icon": "times",
  "prefix": "fa",
  "extraClasses": "fa-rotate-0",
}
            );
        
    
        var popup_63011868b1884435bd3ca50de1e391ad = L.popup({
  "maxWidth": 350,
});

        
            
                var html_ba5ce7779a164d0c5c04e3985810c951 = $(`<div id="html_ba5ce7779a164d0c5c04e3985810c951" style="width: 100.0%; height: 100.0%;">         <b style='font-size:12px'>Khu đô thị Mễ Trì</b><br>         <hr style='margin:3px 0'>         <b>❌ NOT SELECTED</b><br>         ID: Site_90<br>         District: D_11<br>         <br>         <b>🏗️ Infrastructure:</b><br>         • Area: 70 m²<br>         • Grid Power: 1200 kW<br>         • Base Load: 800 kW<br>         • Base Cost: 180,000,000 VND         </div>`)[0];
                popup_63011868b1884435bd3ca50de1e391ad.setContent(html_ba5ce7779a164d0c5c04e3985810c951);
            
        

        marker_bf02b94c217e09a3b4b0fe172672f5c6.bindPopup(popup_63011868b1884435bd3ca50de1e391ad)
        ;

        
    
    
            marker_bf02b94c217e09a3b4b0fe172672f5c6.bindTooltip(
                `<div>
                     Khu đô thị Mễ Trì (❌ NOT SELECTED)
                 </div>`,
                {
  "sticky": true,
}
            );
        
    
                marker_bf02b94c217e09a3b4b0fe172672f5c6.setIcon(icon_4e2cf668b2e2876154b6787b15e25813);
            
    
            var heat_map_db778a2ff2eab7e8f07895f8f3425e77 = L.heatLayer(
                [[21.0375882767599, 105.836016798972], [21.0321415763038, 105.809331852041], [21.0180245263029, 105.816901052041], [21.0238122587712, 105.812943825055], [21.0475545153838, 105.83722099437], [21.0314358642478, 105.814703707863], [21.0324360462316, 105.812491167384], [21.0392996253807, 105.828983750191], [21.0265830829458, 105.85906609437], [21.0261753137041, 105.847323967384], [21.0273403780546, 105.859642931692], [21.0214173062508, 105.861597994369], [21.0249669990316, 105.853306052041], [21.031712291026, 105.846469079027], [21.0246041577598, 105.85154329437], [21.0320277496415, 105.85157569437], [21.010042615067, 105.823861501479], [21.0190785404453, 105.824301509712], [21.0020087704945, 105.823001023204], [21.0102051205881, 105.838166790669], [21.0126971036958, 105.823982780876], [21.0081011573386, 105.82771805204], [21.0037721483514, 105.830583789792], [21.0196704043724, 105.827735107862], [21.0111497989239, 105.849558236698], [20.9934769307658, 105.86855805204], [21.0173985669612, 105.845726767384], [21.0020934059866, 105.840450180876], [20.9998768080708, 105.869868065533], [21.0037361684065, 105.859374994369], [21.0027788732352, 105.861731207862], [20.9964507101763, 105.850167336697], [20.967999474924, 105.826531384399], [20.9659561450827, 105.8424142304], [20.9834906852909, 105.85757955389], [20.9646313273372, 105.854585521353], [20.9853406429572, 105.84671735574], [20.9645698744618, 105.822642055303], [20.9749409928213, 105.825652609285], [20.9811157015231, 105.841989999697], [21.0033551688671, 105.815410579026], [20.9988674508698, 105.796473057468], [20.9871406789402, 105.796355008673], [21.0019411811774, 105.823011757468], [21.0030219494811, 105.797524438121], [20.9998415381356, 105.807610136275], [20.995556528672, 105.804596378605], [20.9804716313407, 105.814821769484], [21.0072439672541, 105.795750526984], [21.0075594201988, 105.793187999999], [21.0359688870967, 105.782779257671], [21.0119845086685, 105.800458784656], [21.0357202152681, 105.794687515343], [21.0195528551574, 105.797446969312], [21.038001138068, 105.782283142328], [21.0509164102781, 105.916429742328], [21.0276161588911, 105.898784871164], [21.0390849948569, 105.894407592328], [21.0411462099288, 105.917765157671], [21.0505406825481, 105.893541813492], [21.0461134153963, 105.866600542328], [21.02170366956, 105.89500131164], [20.9948298145081, 105.760771770592], [20.989964139743, 105.751727628835], [20.9498094312606, 105.747638484658], [20.9589179558431, 105.768850671164], [20.972698557349, 105.758526637798], [20.9632401863197, 105.746182928835], [20.9644466096936, 105.771818528835], [21.0762514334647, 105.812704915341], [21.0759930025875, 105.809941638091], [21.0723619413213, 105.809122169316], [21.0731626037496, 105.817198098152], [21.0610906305142, 105.831916684658], [21.0521750056121, 105.808481528835], [21.0553615255241, 105.819707342329], [21.0723305958316, 105.774014830683], [21.0642191980952, 105.787621915341], [21.0696987120028, 105.797519099999], [21.053246216553, 105.7800935], [21.0396087150024, 105.781930122749], [21.0545963394432, 105.779075284658], [21.0535151723472, 105.775812331529], [21.0154700560823, 105.777696957672], [21.0184959299305, 105.78410135582], [21.0207737453963, 105.765192369312], [21.0058713961374, 105.787638986507], [21.0018388200846, 105.782700169258], [21.0286884862292, 105.777203025132], [21.0147179118105, 105.777807342327]],
                {
  "minOpacity": 0.2,
  "maxZoom": 1,
  "radius": 15,
  "blur": 25,
}
            );
        
    
            heat_map_db778a2ff2eab7e8f07895f8f3425e77.addTo(map_c8ff09de98adc905a54fc2040c1d5971);
        
    
            var circle_d863bbffb0cd6f15ae7eca0626a7f829 = L.circle(
                [21.0273403780546, 105.859642931692],
                {"bubblingMouseEvents": true, "color": "green", "dashArray": null, "dashOffset": null, "fill": true, "fillColor": "green", "fillOpacity": 0.15, "fillRule": "evenodd", "lineCap": "round", "lineJoin": "round", "opacity": 1.0, "radius": 10, "stroke": true, "weight": 2}
            ).addTo(map_c8ff09de98adc905a54fc2040c1d5971);
        
    
        var popup_6c949a69925683ddd27d7f70e61ad89e = L.popup({
  "maxWidth": "100%",
});

        
            
                var html_0108175dd138d0b9991c77585c581f4e = $(`<div id="html_0108175dd138d0b9991c77585c581f4e" style="width: 100.0%; height: 100.0%;">Coverage: DCAR XANH</div>`)[0];
                popup_6c949a69925683ddd27d7f70e61ad89e.setContent(html_0108175dd138d0b9991c77585c581f4e);
            
        

        circle_d863bbffb0cd6f15ae7eca0626a7f829.bindPopup(popup_6c949a69925683ddd27d7f70e61ad89e)
        ;

        
    
    
            var circle_5e2bcce527a62d7d3c7eac72eaac280e = L.circle(
                [21.0273403780546, 105.859642931692],
                {"bubblingMouseEvents": true, "color": "darkgreen", "dashArray": null, "dashOffset": null, "fill": false, "fillColor": "darkgreen", "fillOpacity": 0.2, "fillRule": "evenodd", "lineCap": "round", "lineJoin": "round", "opacity": 0.5, "radius": 600, "stroke": true, "weight": 1}
            ).addTo(map_c8ff09de98adc905a54fc2040c1d5971);
        
    
            var circle_89ee84adf3b0ecf8f5f304c05b0c643f = L.circle(
                [21.0214173062508, 105.861597994369],
                {"bubblingMouseEvents": true, "color": "green", "dashArray": null, "dashOffset": null, "fill": true, "fillColor": "green", "fillOpacity": 0.15, "fillRule": "evenodd", "lineCap": "round", "lineJoin": "round", "opacity": 1.0, "radius": 10, "stroke": true, "weight": 2}
            ).addTo(map_c8ff09de98adc905a54fc2040c1d5971);
        
    
        var popup_6f07b56b06efa7e1f7b097961e787094 = L.popup({
  "maxWidth": "100%",
});

        
            
                var html_61e1e33b9f8627b87e6163326aeed805 = $(`<div id="html_61e1e33b9f8627b87e6163326aeed805" style="width: 100.0%; height: 100.0%;">Coverage: Nhà xe Vấn Quyên</div>`)[0];
                popup_6f07b56b06efa7e1f7b097961e787094.setContent(html_61e1e33b9f8627b87e6163326aeed805);
            
        

        circle_89ee84adf3b0ecf8f5f304c05b0c643f.bindPopup(popup_6f07b56b06efa7e1f7b097961e787094)
        ;

        
    
    
            var circle_7ed66a5b7e3dba183fa90bc4dc9c8606 = L.circle(
                [21.0214173062508, 105.861597994369],
                {"bubblingMouseEvents": true, "color": "darkgreen", "dashArray": null, "dashOffset": null, "fill": false, "fillColor": "darkgreen", "fillOpacity": 0.2, "fillRule": "evenodd", "lineCap": "round", "lineJoin": "round", "opacity": 0.5, "radius": 600, "stroke": true, "weight": 1}
            ).addTo(map_c8ff09de98adc905a54fc2040c1d5971);
        
    
            var circle_49c438b6ac9c753bb8edccb0ecbfad00 = L.circle(
                [21.0190785404453, 105.824301509712],
                {"bubblingMouseEvents": true, "color": "green", "dashArray": null, "dashOffset": null, "fill": true, "fillColor": "green", "fillOpacity": 0.15, "fillRule": "evenodd", "lineCap": "round", "lineJoin": "round", "opacity": 1.0, "radius": 10, "stroke": true, "weight": 2}
            ).addTo(map_c8ff09de98adc905a54fc2040c1d5971);
        
    
        var popup_4248463097cd5a778a4be9109182a7a9 = L.popup({
  "maxWidth": "100%",
});

        
            
                var html_2318b53c4abba17243e74ae8e500dd41 = $(`<div id="html_2318b53c4abba17243e74ae8e500dd41" style="width: 100.0%; height: 100.0%;">Coverage: Bãi gửi xe ở phố Hoàng Cầu</div>`)[0];
                popup_4248463097cd5a778a4be9109182a7a9.setContent(html_2318b53c4abba17243e74ae8e500dd41);
            
        

        circle_49c438b6ac9c753bb8edccb0ecbfad00.bindPopup(popup_4248463097cd5a778a4be9109182a7a9)
        ;

        
    
    
            var circle_69976362da1f8fdd6fcff1ae2b6dd81d = L.circle(
                [21.0190785404453, 105.824301509712],
                {"bubblingMouseEvents": true, "color": "darkgreen", "dashArray": null, "dashOffset": null, "fill": false, "fillColor": "darkgreen", "fillOpacity": 0.2, "fillRule": "evenodd", "lineCap": "round", "lineJoin": "round", "opacity": 0.5, "radius": 600, "stroke": true, "weight": 1}
            ).addTo(map_c8ff09de98adc905a54fc2040c1d5971);
        
    
            var circle_64cc3014972a34ab473c617f4f58a1a3 = L.circle(
                [21.0020087704945, 105.823001023204],
                {"bubblingMouseEvents": true, "color": "green", "dashArray": null, "dashOffset": null, "fill": true, "fillColor": "green", "fillOpacity": 0.15, "fillRule": "evenodd", "lineCap": "round", "lineJoin": "round", "opacity": 1.0, "radius": 10, "stroke": true, "weight": 2}
            ).addTo(map_c8ff09de98adc905a54fc2040c1d5971);
        
    
        var popup_80450a98e05c60e7c610c5ff4d13b729 = L.popup({
  "maxWidth": "100%",
});

        
            
                var html_a0d55d13ac19ea0892ebf29930d5055c = $(`<div id="html_a0d55d13ac19ea0892ebf29930d5055c" style="width: 100.0%; height: 100.0%;">Coverage: Bãi đỗ xe Trường Chinh</div>`)[0];
                popup_80450a98e05c60e7c610c5ff4d13b729.setContent(html_a0d55d13ac19ea0892ebf29930d5055c);
            
        

        circle_64cc3014972a34ab473c617f4f58a1a3.bindPopup(popup_80450a98e05c60e7c610c5ff4d13b729)
        ;

        
    
    
            var circle_faa993e0efd39ea9feee7ebb0f284ee2 = L.circle(
                [21.0020087704945, 105.823001023204],
                {"bubblingMouseEvents": true, "color": "darkgreen", "dashArray": null, "dashOffset": null, "fill": false, "fillColor": "darkgreen", "fillOpacity": 0.2, "fillRule": "evenodd", "lineCap": "round", "lineJoin": "round", "opacity": 0.5, "radius": 600, "stroke": true, "weight": 1}
            ).addTo(map_c8ff09de98adc905a54fc2040c1d5971);
        
    
            var circle_d9b46f40029c02c9604d36f964895141 = L.circle(
                [21.0102051205881, 105.838166790669],
                {"bubblingMouseEvents": true, "color": "green", "dashArray": null, "dashOffset": null, "fill": true, "fillColor": "green", "fillOpacity": 0.15, "fillRule": "evenodd", "lineCap": "round", "lineJoin": "round", "opacity": 1.0, "radius": 10, "stroke": true, "weight": 2}
            ).addTo(map_c8ff09de98adc905a54fc2040c1d5971);
        
    
        var popup_5e6dc6743bf973be4cbd3c831fc74ee0 = L.popup({
  "maxWidth": "100%",
});

        
            
                var html_17916ba021785297135de53277eedebe = $(`<div id="html_17916ba021785297135de53277eedebe" style="width: 100.0%; height: 100.0%;">Coverage: Bãi giữ xe đình Kim Liên</div>`)[0];
                popup_5e6dc6743bf973be4cbd3c831fc74ee0.setContent(html_17916ba021785297135de53277eedebe);
            
        

        circle_d9b46f40029c02c9604d36f964895141.bindPopup(popup_5e6dc6743bf973be4cbd3c831fc74ee0)
        ;

        
    
    
            var circle_79a9181fdc6ed1e094e31538af46ee4a = L.circle(
                [21.0102051205881, 105.838166790669],
                {"bubblingMouseEvents": true, "color": "darkgreen", "dashArray": null, "dashOffset": null, "fill": false, "fillColor": "darkgreen", "fillOpacity": 0.2, "fillRule": "evenodd", "lineCap": "round", "lineJoin": "round", "opacity": 0.5, "radius": 600, "stroke": true, "weight": 1}
            ).addTo(map_c8ff09de98adc905a54fc2040c1d5971);
        
    
            var circle_455cf517efd988db03d78acc5e6682c8 = L.circle(
                [21.0126971036958, 105.823982780876],
                {"bubblingMouseEvents": true, "color": "green", "dashArray": null, "dashOffset": null, "fill": true, "fillColor": "green", "fillOpacity": 0.15, "fillRule": "evenodd", "lineCap": "round", "lineJoin": "round", "opacity": 1.0, "radius": 10, "stroke": true, "weight": 2}
            ).addTo(map_c8ff09de98adc905a54fc2040c1d5971);
        
    
        var popup_098f6ceb1bde170cc295011222270971 = L.popup({
  "maxWidth": "100%",
});

        
            
                var html_4cb22f35922759d2907a41b2961c4328 = $(`<div id="html_4cb22f35922759d2907a41b2961c4328" style="width: 100.0%; height: 100.0%;">Coverage: Công viên Đống Đa</div>`)[0];
                popup_098f6ceb1bde170cc295011222270971.setContent(html_4cb22f35922759d2907a41b2961c4328);
            
        

        circle_455cf517efd988db03d78acc5e6682c8.bindPopup(popup_098f6ceb1bde170cc295011222270971)
        ;

        
    
    
            var circle_c2665b7682a220a6448da22c81894ff7 = L.circle(
                [21.0126971036958, 105.823982780876],
                {"bubblingMouseEvents": true, "color": "darkgreen", "dashArray": null, "dashOffset": null, "fill": false, "fillColor": "darkgreen", "fillOpacity": 0.2, "fillRule": "evenodd", "lineCap": "round", "lineJoin": "round", "opacity": 0.5, "radius": 600, "stroke": true, "weight": 1}
            ).addTo(map_c8ff09de98adc905a54fc2040c1d5971);
        
    
            var circle_b7bb7b192aeebaf18e62b26cd79b08bf = L.circle(
                [21.0081011573386, 105.82771805204],
                {"bubblingMouseEvents": true, "color": "green", "dashArray": null, "dashOffset": null, "fill": true, "fillColor": "green", "fillOpacity": 0.15, "fillRule": "evenodd", "lineCap": "round", "lineJoin": "round", "opacity": 1.0, "radius": 10, "stroke": true, "weight": 2}
            ).addTo(map_c8ff09de98adc905a54fc2040c1d5971);
        
    
        var popup_b76c6e0453d5f3de7c9c1e3f737fc488 = L.popup({
  "maxWidth": "100%",
});

        
            
                var html_012b020233c1e76b9552a5356c6c59ca = $(`<div id="html_012b020233c1e76b9552a5356c6c59ca" style="width: 100.0%; height: 100.0%;">Coverage: P. Chùa Bộc</div>`)[0];
                popup_b76c6e0453d5f3de7c9c1e3f737fc488.setContent(html_012b020233c1e76b9552a5356c6c59ca);
            
        

        circle_b7bb7b192aeebaf18e62b26cd79b08bf.bindPopup(popup_b76c6e0453d5f3de7c9c1e3f737fc488)
        ;

        
    
    
            var circle_da28defad8899d79c3e93fe4184c549c = L.circle(
                [21.0081011573386, 105.82771805204],
                {"bubblingMouseEvents": true, "color": "darkgreen", "dashArray": null, "dashOffset": null, "fill": false, "fillColor": "darkgreen", "fillOpacity": 0.2, "fillRule": "evenodd", "lineCap": "round", "lineJoin": "round", "opacity": 0.5, "radius": 600, "stroke": true, "weight": 1}
            ).addTo(map_c8ff09de98adc905a54fc2040c1d5971);
        
    
            var circle_0aaf66ce8827ddb7b49c9b1b8c3c837a = L.circle(
                [21.0037721483514, 105.830583789792],
                {"bubblingMouseEvents": true, "color": "green", "dashArray": null, "dashOffset": null, "fill": true, "fillColor": "green", "fillOpacity": 0.15, "fillRule": "evenodd", "lineCap": "round", "lineJoin": "round", "opacity": 1.0, "radius": 10, "stroke": true, "weight": 2}
            ).addTo(map_c8ff09de98adc905a54fc2040c1d5971);
        
    
        var popup_d82a176f14f5d4f9a78813a0eae9e8ca = L.popup({
  "maxWidth": "100%",
});

        
            
                var html_bfeaa4cf36467863d914c3c6b866aeb8 = $(`<div id="html_bfeaa4cf36467863d914c3c6b866aeb8" style="width: 100.0%; height: 100.0%;">Coverage: Đại học Y Hà Nội</div>`)[0];
                popup_d82a176f14f5d4f9a78813a0eae9e8ca.setContent(html_bfeaa4cf36467863d914c3c6b866aeb8);
            
        

        circle_0aaf66ce8827ddb7b49c9b1b8c3c837a.bindPopup(popup_d82a176f14f5d4f9a78813a0eae9e8ca)
        ;

        
    
    
            var circle_e8c808800cdaec267cc6302e3b681ae9 = L.circle(
                [21.0037721483514, 105.830583789792],
                {"bubblingMouseEvents": true, "color": "darkgreen", "dashArray": null, "dashOffset": null, "fill": false, "fillColor": "darkgreen", "fillOpacity": 0.2, "fillRule": "evenodd", "lineCap": "round", "lineJoin": "round", "opacity": 0.5, "radius": 600, "stroke": true, "weight": 1}
            ).addTo(map_c8ff09de98adc905a54fc2040c1d5971);
        
    
            var circle_887d6f0966242248ac160a1a7a0c9fd7 = L.circle(
                [20.9934769307658, 105.86855805204],
                {"bubblingMouseEvents": true, "color": "green", "dashArray": null, "dashOffset": null, "fill": true, "fillColor": "green", "fillOpacity": 0.15, "fillRule": "evenodd", "lineCap": "round", "lineJoin": "round", "opacity": 1.0, "radius": 10, "stroke": true, "weight": 2}
            ).addTo(map_c8ff09de98adc905a54fc2040c1d5971);
        
    
        var popup_551a173be89626d3bb5ad1d341d39389 = L.popup({
  "maxWidth": "100%",
});

        
            
                var html_5b515131ffa3c37732266ea16b148e68 = $(`<div id="html_5b515131ffa3c37732266ea16b148e68" style="width: 100.0%; height: 100.0%;">Coverage: Times City T11</div>`)[0];
                popup_551a173be89626d3bb5ad1d341d39389.setContent(html_5b515131ffa3c37732266ea16b148e68);
            
        

        circle_887d6f0966242248ac160a1a7a0c9fd7.bindPopup(popup_551a173be89626d3bb5ad1d341d39389)
        ;

        
    
    
            var circle_8dc9287aff7c6a4a1761e08e4adabb5e = L.circle(
                [20.9934769307658, 105.86855805204],
                {"bubblingMouseEvents": true, "color": "darkgreen", "dashArray": null, "dashOffset": null, "fill": false, "fillColor": "darkgreen", "fillOpacity": 0.2, "fillRule": "evenodd", "lineCap": "round", "lineJoin": "round", "opacity": 0.5, "radius": 600, "stroke": true, "weight": 1}
            ).addTo(map_c8ff09de98adc905a54fc2040c1d5971);
        
    
            var circle_09dd7b773caf1c96f8e618cc490c7c79 = L.circle(
                [20.9998768080708, 105.869868065533],
                {"bubblingMouseEvents": true, "color": "green", "dashArray": null, "dashOffset": null, "fill": true, "fillColor": "green", "fillOpacity": 0.15, "fillRule": "evenodd", "lineCap": "round", "lineJoin": "round", "opacity": 1.0, "radius": 10, "stroke": true, "weight": 2}
            ).addTo(map_c8ff09de98adc905a54fc2040c1d5971);
        
    
        var popup_5a663daa18427317f286cf5a9612b378 = L.popup({
  "maxWidth": "100%",
});

        
            
                var html_31a9a99ef38c0ca8eec282259165cf36 = $(`<div id="html_31a9a99ef38c0ca8eec282259165cf36" style="width: 100.0%; height: 100.0%;">Coverage: Hòa Bình Green City</div>`)[0];
                popup_5a663daa18427317f286cf5a9612b378.setContent(html_31a9a99ef38c0ca8eec282259165cf36);
            
        

        circle_09dd7b773caf1c96f8e618cc490c7c79.bindPopup(popup_5a663daa18427317f286cf5a9612b378)
        ;

        
    
    
            var circle_8a8de932c595606235796cddf161d589 = L.circle(
                [20.9998768080708, 105.869868065533],
                {"bubblingMouseEvents": true, "color": "darkgreen", "dashArray": null, "dashOffset": null, "fill": false, "fillColor": "darkgreen", "fillOpacity": 0.2, "fillRule": "evenodd", "lineCap": "round", "lineJoin": "round", "opacity": 0.5, "radius": 600, "stroke": true, "weight": 1}
            ).addTo(map_c8ff09de98adc905a54fc2040c1d5971);
        
    
            var circle_5dd8807dae14a7617f6d5bfd9773a157 = L.circle(
                [20.9659561450827, 105.8424142304],
                {"bubblingMouseEvents": true, "color": "green", "dashArray": null, "dashOffset": null, "fill": true, "fillColor": "green", "fillOpacity": 0.15, "fillRule": "evenodd", "lineCap": "round", "lineJoin": "round", "opacity": 1.0, "radius": 10, "stroke": true, "weight": 2}
            ).addTo(map_c8ff09de98adc905a54fc2040c1d5971);
        
    
        var popup_c7b93a8361c5c4343f75ede62c96c712 = L.popup({
  "maxWidth": "100%",
});

        
            
                var html_66154929aaa5ba80ce1fa882ed64a575 = $(`<div id="html_66154929aaa5ba80ce1fa882ed64a575" style="width: 100.0%; height: 100.0%;">Coverage: Bến xe Nước Ngầm</div>`)[0];
                popup_c7b93a8361c5c4343f75ede62c96c712.setContent(html_66154929aaa5ba80ce1fa882ed64a575);
            
        

        circle_5dd8807dae14a7617f6d5bfd9773a157.bindPopup(popup_c7b93a8361c5c4343f75ede62c96c712)
        ;

        
    
    
            var circle_ae8544acf22b38c68c5f5e06a6f70cc6 = L.circle(
                [20.9659561450827, 105.8424142304],
                {"bubblingMouseEvents": true, "color": "darkgreen", "dashArray": null, "dashOffset": null, "fill": false, "fillColor": "darkgreen", "fillOpacity": 0.2, "fillRule": "evenodd", "lineCap": "round", "lineJoin": "round", "opacity": 0.5, "radius": 600, "stroke": true, "weight": 1}
            ).addTo(map_c8ff09de98adc905a54fc2040c1d5971);
        
    
            var circle_7802800e99ee55c7f5fcc9fcaee992ce = L.circle(
                [20.9834906852909, 105.85757955389],
                {"bubblingMouseEvents": true, "color": "green", "dashArray": null, "dashOffset": null, "fill": true, "fillColor": "green", "fillOpacity": 0.15, "fillRule": "evenodd", "lineCap": "round", "lineJoin": "round", "opacity": 1.0, "radius": 10, "stroke": true, "weight": 2}
            ).addTo(map_c8ff09de98adc905a54fc2040c1d5971);
        
    
        var popup_1494bf5995e0fc1bf97b1e44df119d8f = L.popup({
  "maxWidth": "100%",
});

        
            
                var html_940ec13cde924f072f2b35ed5910aba3 = $(`<div id="html_940ec13cde924f072f2b35ed5910aba3" style="width: 100.0%; height: 100.0%;">Coverage: Đền Lừ</div>`)[0];
                popup_1494bf5995e0fc1bf97b1e44df119d8f.setContent(html_940ec13cde924f072f2b35ed5910aba3);
            
        

        circle_7802800e99ee55c7f5fcc9fcaee992ce.bindPopup(popup_1494bf5995e0fc1bf97b1e44df119d8f)
        ;

        
    
    
            var circle_0688be870818d8ef31b9bc3412843dc6 = L.circle(
                [20.9834906852909, 105.85757955389],
                {"bubblingMouseEvents": true, "color": "darkgreen", "dashArray": null, "dashOffset": null, "fill": false, "fillColor": "darkgreen", "fillOpacity": 0.2, "fillRule": "evenodd", "lineCap": "round", "lineJoin": "round", "opacity": 0.5, "radius": 600, "stroke": true, "weight": 1}
            ).addTo(map_c8ff09de98adc905a54fc2040c1d5971);
        
    
            var circle_89feab172400b97dfd60de9cf7717fd0 = L.circle(
                [20.9804716313407, 105.814821769484],
                {"bubblingMouseEvents": true, "color": "green", "dashArray": null, "dashOffset": null, "fill": true, "fillColor": "green", "fillOpacity": 0.15, "fillRule": "evenodd", "lineCap": "round", "lineJoin": "round", "opacity": 1.0, "radius": 10, "stroke": true, "weight": 2}
            ).addTo(map_c8ff09de98adc905a54fc2040c1d5971);
        
    
        var popup_d96657c18f7583e8a58d8fd1dfbe7cad = L.popup({
  "maxWidth": "100%",
});

        
            
                var html_1d284c0f1767d37c03ab4395011901af = $(`<div id="html_1d284c0f1767d37c03ab4395011901af" style="width: 100.0%; height: 100.0%;">Coverage: Bãi đỗ xe Kim Giang</div>`)[0];
                popup_d96657c18f7583e8a58d8fd1dfbe7cad.setContent(html_1d284c0f1767d37c03ab4395011901af);
            
        

        circle_89feab172400b97dfd60de9cf7717fd0.bindPopup(popup_d96657c18f7583e8a58d8fd1dfbe7cad)
        ;

        
    
    
            var circle_da773eb15d58997a37ce4e4852335c90 = L.circle(
                [20.9804716313407, 105.814821769484],
                {"bubblingMouseEvents": true, "color": "darkgreen", "dashArray": null, "dashOffset": null, "fill": false, "fillColor": "darkgreen", "fillOpacity": 0.2, "fillRule": "evenodd", "lineCap": "round", "lineJoin": "round", "opacity": 0.5, "radius": 600, "stroke": true, "weight": 1}
            ).addTo(map_c8ff09de98adc905a54fc2040c1d5971);
        
    
            var circle_cb7a489d372c750e81efe0a075f37482 = L.circle(
                [21.0195528551574, 105.797446969312],
                {"bubblingMouseEvents": true, "color": "green", "dashArray": null, "dashOffset": null, "fill": true, "fillColor": "green", "fillOpacity": 0.15, "fillRule": "evenodd", "lineCap": "round", "lineJoin": "round", "opacity": 1.0, "radius": 10, "stroke": true, "weight": 2}
            ).addTo(map_c8ff09de98adc905a54fc2040c1d5971);
        
    
        var popup_ccca6a7c62ec24eabe3850c9cdd8dd50 = L.popup({
  "maxWidth": "100%",
});

        
            
                var html_3cb72061c2d0257dd816910a58ef183b = $(`<div id="html_3cb72061c2d0257dd816910a58ef183b" style="width: 100.0%; height: 100.0%;">Coverage: Khu đô thị Yên Hòa</div>`)[0];
                popup_ccca6a7c62ec24eabe3850c9cdd8dd50.setContent(html_3cb72061c2d0257dd816910a58ef183b);
            
        

        circle_cb7a489d372c750e81efe0a075f37482.bindPopup(popup_ccca6a7c62ec24eabe3850c9cdd8dd50)
        ;

        
    
    
            var circle_a3af54cd6cffe7dfebd9f6117adc0a9f = L.circle(
                [21.0195528551574, 105.797446969312],
                {"bubblingMouseEvents": true, "color": "darkgreen", "dashArray": null, "dashOffset": null, "fill": false, "fillColor": "darkgreen", "fillOpacity": 0.2, "fillRule": "evenodd", "lineCap": "round", "lineJoin": "round", "opacity": 0.5, "radius": 600, "stroke": true, "weight": 1}
            ).addTo(map_c8ff09de98adc905a54fc2040c1d5971);
        
    
            var circle_01679effa141c5e88bb34fc10c6d3b46 = L.circle(
                [21.0390849948569, 105.894407592328],
                {"bubblingMouseEvents": true, "color": "green", "dashArray": null, "dashOffset": null, "fill": true, "fillColor": "green", "fillOpacity": 0.15, "fillRule": "evenodd", "lineCap": "round", "lineJoin": "round", "opacity": 1.0, "radius": 10, "stroke": true, "weight": 2}
            ).addTo(map_c8ff09de98adc905a54fc2040c1d5971);
        
    
        var popup_41caf13484380a037cb057d3e2def991 = L.popup({
  "maxWidth": "100%",
});

        
            
                var html_26df13d0a4923b669ece64496759cd98 = $(`<div id="html_26df13d0a4923b669ece64496759cd98" style="width: 100.0%; height: 100.0%;">Coverage: Bãi đỗ xe Sân Golf Long Biên</div>`)[0];
                popup_41caf13484380a037cb057d3e2def991.setContent(html_26df13d0a4923b669ece64496759cd98);
            
        

        circle_01679effa141c5e88bb34fc10c6d3b46.bindPopup(popup_41caf13484380a037cb057d3e2def991)
        ;

        
    
    
            var circle_13cd89df19a81d2e52e3f2ae39e86ea3 = L.circle(
                [21.0390849948569, 105.894407592328],
                {"bubblingMouseEvents": true, "color": "darkgreen", "dashArray": null, "dashOffset": null, "fill": false, "fillColor": "darkgreen", "fillOpacity": 0.2, "fillRule": "evenodd", "lineCap": "round", "lineJoin": "round", "opacity": 0.5, "radius": 600, "stroke": true, "weight": 1}
            ).addTo(map_c8ff09de98adc905a54fc2040c1d5971);
        
    
            var circle_4639e7fe019b1178f3491644aa4c7218 = L.circle(
                [21.02170366956, 105.89500131164],
                {"bubblingMouseEvents": true, "color": "green", "dashArray": null, "dashOffset": null, "fill": true, "fillColor": "green", "fillOpacity": 0.15, "fillRule": "evenodd", "lineCap": "round", "lineJoin": "round", "opacity": 1.0, "radius": 10, "stroke": true, "weight": 2}
            ).addTo(map_c8ff09de98adc905a54fc2040c1d5971);
        
    
        var popup_aa0cc79af6677d6780cc7a341e2e9ca8 = L.popup({
  "maxWidth": "100%",
});

        
            
                var html_80bb45c8be8cad376be7aa8a4724ace0 = $(`<div id="html_80bb45c8be8cad376be7aa8a4724ace0" style="width: 100.0%; height: 100.0%;">Coverage: Bãi xe Cầu Vĩnh Tuy</div>`)[0];
                popup_aa0cc79af6677d6780cc7a341e2e9ca8.setContent(html_80bb45c8be8cad376be7aa8a4724ace0);
            
        

        circle_4639e7fe019b1178f3491644aa4c7218.bindPopup(popup_aa0cc79af6677d6780cc7a341e2e9ca8)
        ;

        
    
    
            var circle_cf984aff6b2eb0d3caf19d1ef5abf2be = L.circle(
                [21.02170366956, 105.89500131164],
                {"bubblingMouseEvents": true, "color": "darkgreen", "dashArray": null, "dashOffset": null, "fill": false, "fillColor": "darkgreen", "fillOpacity": 0.2, "fillRule": "evenodd", "lineCap": "round", "lineJoin": "round", "opacity": 0.5, "radius": 600, "stroke": true, "weight": 1}
            ).addTo(map_c8ff09de98adc905a54fc2040c1d5971);
        
    
            var circle_0f4c51da2e944c68d4832475fdd65f28 = L.circle(
                [20.9632401863197, 105.746182928835],
                {"bubblingMouseEvents": true, "color": "green", "dashArray": null, "dashOffset": null, "fill": true, "fillColor": "green", "fillOpacity": 0.15, "fillRule": "evenodd", "lineCap": "round", "lineJoin": "round", "opacity": 1.0, "radius": 10, "stroke": true, "weight": 2}
            ).addTo(map_c8ff09de98adc905a54fc2040c1d5971);
        
    
        var popup_a85482229554a86514adc5f2c0db666a = L.popup({
  "maxWidth": "100%",
});

        
            
                var html_70c4277f74d0acf93e1b3587d5693bb6 = $(`<div id="html_70c4277f74d0acf93e1b3587d5693bb6" style="width: 100.0%; height: 100.0%;">Coverage: Khu đô thị Dương Nội</div>`)[0];
                popup_a85482229554a86514adc5f2c0db666a.setContent(html_70c4277f74d0acf93e1b3587d5693bb6);
            
        

        circle_0f4c51da2e944c68d4832475fdd65f28.bindPopup(popup_a85482229554a86514adc5f2c0db666a)
        ;

        
    
    
            var circle_1b919483d16c964c13344f134b0f0317 = L.circle(
                [20.9632401863197, 105.746182928835],
                {"bubblingMouseEvents": true, "color": "darkgreen", "dashArray": null, "dashOffset": null, "fill": false, "fillColor": "darkgreen", "fillOpacity": 0.2, "fillRule": "evenodd", "lineCap": "round", "lineJoin": "round", "opacity": 0.5, "radius": 600, "stroke": true, "weight": 1}
            ).addTo(map_c8ff09de98adc905a54fc2040c1d5971);
        
    
            var circle_1a27ff202c565dd22327c904171ee532 = L.circle(
                [21.0759930025875, 105.809941638091],
                {"bubblingMouseEvents": true, "color": "green", "dashArray": null, "dashOffset": null, "fill": true, "fillColor": "green", "fillOpacity": 0.15, "fillRule": "evenodd", "lineCap": "round", "lineJoin": "round", "opacity": 1.0, "radius": 10, "stroke": true, "weight": 2}
            ).addTo(map_c8ff09de98adc905a54fc2040c1d5971);
        
    
        var popup_f029a35d7e0e65338a60428a5060ac54 = L.popup({
  "maxWidth": "100%",
});

        
            
                var html_4170eacdee4e283d4e442ddd9c0a73aa = $(`<div id="html_4170eacdee4e283d4e442ddd9c0a73aa" style="width: 100.0%; height: 100.0%;">Coverage: Ciputra Parking Complex</div>`)[0];
                popup_f029a35d7e0e65338a60428a5060ac54.setContent(html_4170eacdee4e283d4e442ddd9c0a73aa);
            
        

        circle_1a27ff202c565dd22327c904171ee532.bindPopup(popup_f029a35d7e0e65338a60428a5060ac54)
        ;

        
    
    
            var circle_9f07d02293e5112cf6b6b36bdb6bc3e5 = L.circle(
                [21.0759930025875, 105.809941638091],
                {"bubblingMouseEvents": true, "color": "darkgreen", "dashArray": null, "dashOffset": null, "fill": false, "fillColor": "darkgreen", "fillOpacity": 0.2, "fillRule": "evenodd", "lineCap": "round", "lineJoin": "round", "opacity": 0.5, "radius": 600, "stroke": true, "weight": 1}
            ).addTo(map_c8ff09de98adc905a54fc2040c1d5971);
        
    
            var circle_68947f5861bf8eca0743007627068bae = L.circle(
                [21.0723305958316, 105.774014830683],
                {"bubblingMouseEvents": true, "color": "green", "dashArray": null, "dashOffset": null, "fill": true, "fillColor": "green", "fillOpacity": 0.15, "fillRule": "evenodd", "lineCap": "round", "lineJoin": "round", "opacity": 1.0, "radius": 10, "stroke": true, "weight": 2}
            ).addTo(map_c8ff09de98adc905a54fc2040c1d5971);
        
    
        var popup_378d7fbe6232bd87849b6f9d4a80fa0f = L.popup({
  "maxWidth": "100%",
});

        
            
                var html_112147bbdca149795031cf755e3aa36d = $(`<div id="html_112147bbdca149795031cf755e3aa36d" style="width: 100.0%; height: 100.0%;">Coverage: Đại học Mỏ Địa Chất Parking</div>`)[0];
                popup_378d7fbe6232bd87849b6f9d4a80fa0f.setContent(html_112147bbdca149795031cf755e3aa36d);
            
        

        circle_68947f5861bf8eca0743007627068bae.bindPopup(popup_378d7fbe6232bd87849b6f9d4a80fa0f)
        ;

        
    
    
            var circle_dc61d14f43ee1c503ee9f3da66bd3dde = L.circle(
                [21.0723305958316, 105.774014830683],
                {"bubblingMouseEvents": true, "color": "darkgreen", "dashArray": null, "dashOffset": null, "fill": false, "fillColor": "darkgreen", "fillOpacity": 0.2, "fillRule": "evenodd", "lineCap": "round", "lineJoin": "round", "opacity": 0.5, "radius": 600, "stroke": true, "weight": 1}
            ).addTo(map_c8ff09de98adc905a54fc2040c1d5971);
        
    
            var circle_d9b4729f8088baf49478feb1a2cefb34 = L.circle(
                [21.053246216553, 105.7800935],
                {"bubblingMouseEvents": true, "color": "green", "dashArray": null, "dashOffset": null, "fill": true, "fillColor": "green", "fillOpacity": 0.15, "fillRule": "evenodd", "lineCap": "round", "lineJoin": "round", "opacity": 1.0, "radius": 10, "stroke": true, "weight": 2}
            ).addTo(map_c8ff09de98adc905a54fc2040c1d5971);
        
    
        var popup_6965731d90015b271eb53ddeacc92334 = L.popup({
  "maxWidth": "100%",
});

        
            
                var html_076a43dece8311a0fd1f08a7934f9fa4 = $(`<div id="html_076a43dece8311a0fd1f08a7934f9fa4" style="width: 100.0%; height: 100.0%;">Coverage: Chung cư Green Stars</div>`)[0];
                popup_6965731d90015b271eb53ddeacc92334.setContent(html_076a43dece8311a0fd1f08a7934f9fa4);
            
        

        circle_d9b4729f8088baf49478feb1a2cefb34.bindPopup(popup_6965731d90015b271eb53ddeacc92334)
        ;

        
    
    
            var circle_cfded0b06d4fb0244538a3b57716ee2f = L.circle(
                [21.053246216553, 105.7800935],
                {"bubblingMouseEvents": true, "color": "darkgreen", "dashArray": null, "dashOffset": null, "fill": false, "fillColor": "darkgreen", "fillOpacity": 0.2, "fillRule": "evenodd", "lineCap": "round", "lineJoin": "round", "opacity": 0.5, "radius": 600, "stroke": true, "weight": 1}
            ).addTo(map_c8ff09de98adc905a54fc2040c1d5971);
        
    
            var circle_43b413c54fdebbe8cb7d94b60eeed01c = L.circle(
                [21.0154700560823, 105.777696957672],
                {"bubblingMouseEvents": true, "color": "green", "dashArray": null, "dashOffset": null, "fill": true, "fillColor": "green", "fillOpacity": 0.15, "fillRule": "evenodd", "lineCap": "round", "lineJoin": "round", "opacity": 1.0, "radius": 10, "stroke": true, "weight": 2}
            ).addTo(map_c8ff09de98adc905a54fc2040c1d5971);
        
    
        var popup_df5b232a1ea33107ab72ddb38a9c3715 = L.popup({
  "maxWidth": "100%",
});

        
            
                var html_ddbba66ebe03c7f753efca3f3072e7a6 = $(`<div id="html_ddbba66ebe03c7f753efca3f3072e7a6" style="width: 100.0%; height: 100.0%;">Coverage: Vincom Plaza The Garden</div>`)[0];
                popup_df5b232a1ea33107ab72ddb38a9c3715.setContent(html_ddbba66ebe03c7f753efca3f3072e7a6);
            
        

        circle_43b413c54fdebbe8cb7d94b60eeed01c.bindPopup(popup_df5b232a1ea33107ab72ddb38a9c3715)
        ;

        
    
    
            var circle_3978afa36dad7bf9cdc76ac28d33a94b = L.circle(
                [21.0154700560823, 105.777696957672],
                {"bubblingMouseEvents": true, "color": "darkgreen", "dashArray": null, "dashOffset": null, "fill": false, "fillColor": "darkgreen", "fillOpacity": 0.2, "fillRule": "evenodd", "lineCap": "round", "lineJoin": "round", "opacity": 0.5, "radius": 600, "stroke": true, "weight": 1}
            ).addTo(map_c8ff09de98adc905a54fc2040c1d5971);
        
    
            var layer_control_28bb6609c633ea121cf2ee6ace8c7d6c_layers = {
                base_layers : {
                    "openstreetmap" : tile_layer_d949b83fe6f517e896e0f6c4843cfe36,
                },
                overlays :  {
                    "macro_element_db778a2ff2eab7e8f07895f8f3425e77" : heat_map_db778a2ff2eab7e8f07895f8f3425e77,
                },
            };
            let layer_control_28bb6609c633ea121cf2ee6ace8c7d6c = L.control.layers(
                layer_control_28bb6609c633ea121cf2ee6ace8c7d6c_layers.base_layers,
                layer_control_28bb6609c633ea121cf2ee6ace8c7d6c_layers.overlays,
                {
  "position": "topright",
  "collapsed": true,
  "autoZIndex": true,
}
            ).addTo(map_c8ff09de98adc905a54fc2040c1d5971);

        
    
            tile_layer_d949b83fe6f517e896e0f6c4843cfe36.addTo(map_c8ff09de98adc905a54fc2040c1d5971);
        
    
                marker_3f590acaa38af967496d4a7ce6812e2d.setIcon(icon_dc18ad97906d87525feafb6f7338a80f);
            
    
                marker_a4f037c05a25ab49df8b4d4f8a667c03.setIcon(icon_78b78dec73b94a4b97df30541615ddca);
            
    
                marker_6b26c5a53a2f2faff66663655f121530.setIcon(icon_3b17e3016a68f53730cba3764dab00bd);
            
    
                marker_883bdb94a7a510089568ebdf0d4437ab.setIcon(icon_006e6cc4d6e6d42f911102bb0ae41acc);
            
    
                marker_0a5cd92c6a16602f820d194f95b967e7.setIcon(icon_972bebacfb988009634eca6257aaa943);
            
    
                marker_426697160fc0a77af0ff09c827faea74.setIcon(icon_d5cc3d9a67f425ce3cc7dc5e71bc19e8);
            
    
                marker_43922b55ef8ba27a0f31186a843d91f0.setIcon(icon_f5898716e913f98d632c6069656e1fc9);
            
    
                marker_cd764ee12ad01bb53361441af6fddcc6.setIcon(icon_06292034c9a541eb0c78c8f29ed1b0ee);
            
    
                marker_07e2b95a9383be5b98fc67d2738f4c4c.setIcon(icon_988a57e5383301672753ae8d5b15b2a6);
            
    
                marker_d59f678ad823ae46a2d13dc213f724a1.setIcon(icon_f7ca778969f1c0a7f404222101b8deea);
            
    
                marker_f9e95da173141cba6954fb925ab74b6c.setIcon(icon_8c077bc2b623f9a4a62ec2436ab0a4e1);
            
    
                marker_80e950de2e62359a11fdbcea3f560306.setIcon(icon_6d9f5ade1a4552837272496ce43556e8);
            
    
                marker_86b7bb78898a1126da69cad5fc36fbb9.setIcon(icon_1cdc0b3604a6a407159ba48327427460);
            
    
                marker_d9fcf67510ac995ee8feb7fd1cf0faac.setIcon(icon_5766ef07b6f32f445fa678050bd71b0b);
            
    
                marker_a3197058f827c89bb544c195b110d29d.setIcon(icon_4a423552a90e44a2501136918e3a7477);
            
    
                marker_487022e61230dd5382ed4bd55ff7f856.setIcon(icon_92d62aa9771b073e215117119bc7e0e2);
            
    
                marker_61e71553d595c8fc70c048a78aec7bf7.setIcon(icon_15916f2a36ba01a2468b63988809ec79);
            
    
                marker_cc366cc5c0dbc720e56ba26201d24a70.setIcon(icon_11d1d47a1d40bdfe47983f206d17dcfa);
            
    
                marker_0606b88ee6ce5ceadfd5a41dcf1a23e9.setIcon(icon_cd0ee7bf0fd5ffc72c5b72fd9788a9ee);
            
    
                marker_3a705c43f4dbae8f6189c9f6bd32c09e.setIcon(icon_a626de325cd6302ef1bb1b1b9aa659ab);
            
    
                marker_8dfadf481ecd767e16dd04703e28ec5e.setIcon(icon_480fbe548c59fd152d5d085fc12ac801);
            
    
                marker_3455a3d00352255e1eb471ba0d382ede.setIcon(icon_06c5e247461c3ea62578f6373744df8c);
            
    
                marker_2355a695a3d88d026b841bd22ea0a44e.setIcon(icon_ab833ad763a138f5ee8d96575ea59b46);
            
    
                marker_a3f49352460b89f4fdc394074f42e2e7.setIcon(icon_12e9936a531e94fd5e9d3cee5b4dec1c);
            
    
                marker_523ef938ffb23df9c11e46286bdc2e4b.setIcon(icon_cd9d427f314db9f8c6c08dd476d0340d);
            
    
                marker_885943c0ea96f4a7f6965abe070c72d6.setIcon(icon_c257715adb55c61141bcd5f695f262dc);
            
    
                marker_270e0c6e8a4ea4c23a3579004f5423e5.setIcon(icon_1ea70883537a503a3dd5ec0b66d1aec3);
            
    
                marker_948462a8c8d27a8bead3da64952daa6d.setIcon(icon_8d24760a5a7981e155f8e4a7eb5c47ff);
            
    
                marker_dfeec41f6747008be4aaf1586357d33c.setIcon(icon_5b8961a4f133b510b11981cf7fb3641f);
            
    
                marker_b49f189ced40063eb198ed35de03d024.setIcon(icon_ac0d2c327770a002b45bb22b2692df1f);
            
    
                marker_93313a11aba2910ae2fb886c153a9210.setIcon(icon_42117a88413ed67f06f7432ded10fe69);
            
    
                marker_29130ddb478c66fbdb15d58415791fef.setIcon(icon_2edf867646ac0714c89eed1bb9e52803);
            
    
                marker_6d05676032c49e607aea6663cce5d37c.setIcon(icon_6198fce652fc5ef92a5b6bdb1c3d5d45);
            
    
                marker_19c9d3afb6aad5c11cc7d4a3135cebf0.setIcon(icon_63305b3e13c831cd6e1914782e0bb626);
            
    
                marker_23cd245039ee7571c0efbc63ca0594b2.setIcon(icon_09fb6ad2f21d89a48230b8339a89707f);
            
    
                marker_cd2992d1a1e422de2f7a743aa470deb7.setIcon(icon_18ed817925df8cb5ab575dd4b436f70a);
            
    
                marker_5166b9d2106bd1dfa8a594cc2cdce773.setIcon(icon_6540bdd7aeee829574dc09ecfe8127cd);
            
    
                marker_230e83a44550f779871f328527e1a7c6.setIcon(icon_d71140e589b0008f193280746f88c767);
            
    
                marker_44700b15946f2c45142a56b3b58b2f7b.setIcon(icon_440cc7e3da7eb5dea4859dbe127a308a);
            
    
                marker_d440f326e39957b309d2ecfe725fa50a.setIcon(icon_6f7b3be33ea4d0f6cec4015bfece332d);
            
    
                marker_9280a5f457be8c5faaae181efe1f406e.setIcon(icon_f0ccee8d31a39d9fd01ba658bc72ef94);
            
    
                marker_571a1a42b8f1dc2a2990a5613b94d545.setIcon(icon_838798fa0a21290874c30c35228b4fcf);
            
    
                marker_52e09b4f2ab34c4526a772e2f22aaaab.setIcon(icon_72c9807d85b0fa2f1b7b4d4f36281862);
            
    
                marker_1a373d2474965bba0ebd9dfc59f82625.setIcon(icon_435f95e3e167d1e74d94a1679b2d5404);
            
    
                marker_96c9381721b8cdfb9ec02c447577ec79.setIcon(icon_d06070aea1b38ebd363510d20e146800);
            
    
                marker_7d82b8e756fec4f491a6bdbbfe5f0b68.setIcon(icon_c7b05e6bb23107e3b575a5ba81b6c622);
            
    
                marker_0ca06a8a9a77cde85e964e44ac38cca5.setIcon(icon_b4d04f32c7c36e95251f65a957b1ea71);
            
    
                marker_6a70d51d00aa17fd1428fe6126711c65.setIcon(icon_c44be28ae9969a9e620e2f09efbf630f);
            
    
                marker_111987d43e2e7d0ef1ad3f190b1a8d60.setIcon(icon_24487bc7c70da498ad3565edad11d1e1);
            
    
                marker_832e5a8df64b158fcae2284f69ad00af.setIcon(icon_23c9dcd84d1086bdeff00907efdcb9ca);
            
    
                marker_f000f0b2f2f850268faccb1a26738a2a.setIcon(icon_966ad09b0dfcfdaa5a0842da70a331ac);
            
    
                marker_58cbe95711a9b5d33ba4744c94919eea.setIcon(icon_9b2814a157a58b4b1e7a54de599625a1);
            
    
                marker_8be7e6c3da0f62cb2b554ff26d421088.setIcon(icon_64d0e49bf5a3fe38c19b879a31dc15f8);
            
    
                marker_0a42340b37b71bec5ecc9c7b522a8114.setIcon(icon_ddd8bf1aacd6af0b11435de717def930);
            
    
                marker_04410cfb1fd03a9687fdb67aa107ac0a.setIcon(icon_a6e9326734b73fe90b4b8ba95e22fb68);
            
    
                marker_026790a28da075b50ed66d0317c22a48.setIcon(icon_4f67843e2a48729be6e8dde9e2f85186);
            
    
                marker_c89d1548a3acbb850f7cea7e71b316fe.setIcon(icon_769c1c0a13fdf8623b213e57b0611752);
            
    
                marker_3402447f031eb12dc69a14395dcb04df.setIcon(icon_0f7a58fdb08b510f6aa186da5355b22f);
            
    
                marker_37a9e816cbe54ad4458f989295bb4a4d.setIcon(icon_44b27971918149696bb29828de1519e6);
            
    
                marker_80b52283ba24af338208ac1649e28d49.setIcon(icon_076db85b550048fb937fde4fc9946b93);
            
    
                marker_a3a304dfcb376c3afc464ed1b31677fc.setIcon(icon_fe3c3f1442d2f2e90157a82e333e00fa);
            
    
                marker_ee81207fe12c33b1ffbae49b5f76bbf6.setIcon(icon_6e58629d83dab2366f208a31e5e76f47);
            
    
                marker_4fa223fd0f691b4b122c33c4aa0ec047.setIcon(icon_7a73e2d7c4eb76a18cd56995d68133cc);
            
    
                marker_972ecab2d5cf5031f6b09ad532b34835.setIcon(icon_8a63ed2bb38d1f03ed32459b7c55b21a);
            
    
                marker_f8bdb4bcf77e304c69bc1ae87ce2b28d.setIcon(icon_83085ce02c34423f7e2a81a8e4a35785);
            
    
                marker_68377d78b2f8030063487a22217262d3.setIcon(icon_0ccfa41473ba50569d31a133ab3c291e);
            
    
                marker_35b1baf669cb5a32c092567b9699ad15.setIcon(icon_2a0f0a57a85f7c68bf866141be463574);
            
    
                marker_2006d49cbef7b9eec684a9b222550d7b.setIcon(icon_d631429be6e03f682419616c192b37f6);
            
    
                marker_2f1b99b156b9dc3cd7be1eec10d2eec2.setIcon(icon_cc9ab042445a62eed1c7884a97620536);
            
    
                marker_edecf5ed21156bd7b6e3e04ab96bb1e7.setIcon(icon_97ed0db7e862c1649a88178eb0c19b0c);
            
    
                marker_fe9f7d01595836dabfe5852f06f58873.setIcon(icon_9bd793c1cabf4394dee9f4e972999b90);
            
    
                marker_34fedc988d54a1fb1ae610661c007dc2.setIcon(icon_7e11d665dc56962cd509799d493c67a3);
            
    
                marker_36126a261aae9eb1b55847a5422a148b.setIcon(icon_9b180d7a045a8c3f8a2ac814a4ce402b);
            
    
                marker_f5e5f7df69dbf1aee32bab61e655b166.setIcon(icon_a1a8a41706ce4de5159fa120186079b9);
            
    
                marker_5e6a671374464638c603f1562926bf4f.setIcon(icon_26c18767f238c9693b636274491ace6b);
            
    
                marker_b6090a01162ad3b1c61e5dc8710f32e8.setIcon(icon_cad434cec9f23721e65896ad9e26132e);
            
    
                marker_1dc43eab709063b970ccb25f27aa8a61.setIcon(icon_d3d85b21bf5d48c72bb835089ab921a7);
            
    
                marker_8b843c7b7882ae31e15d0cc0ab9a8e92.setIcon(icon_d4df04fe19e5898d5a6deb910924989c);
            
    
                marker_cfa12262e38d5a4b670f38162aae5c14.setIcon(icon_f78195e4e5acc8e39a9cd1bb67b53f05);
            
    
                marker_337b69dda4af2166ce6c1aec5fed529c.setIcon(icon_bf6bce2f5d9c98c515b0f1c387e288e0);
            
    
                marker_6788e17e1cfd2b794853866f52ed822a.setIcon(icon_861c30eeeb95fdae83148d1b636306f8);
            
    
                marker_3a535b0c2787cd5d7fdf80d412f4bd16.setIcon(icon_055c6f95e2625ed41f137d5287c4e3c4);
            
    
                marker_b2cbf593196a58236bfe392270b5c87e.setIcon(icon_3cf91eba70c4769f9f388968dd06788c);
            
    
                marker_0111f9504e523a0cb15ae333ee53c051.setIcon(icon_e70368ee1aa02912855ec1ec238adc45);
            
    
                marker_6c143d9b2d0681a578cec5d3358d7a47.setIcon(icon_f9b6dae57e9cc94f446ce6a909c9fa16);
            
    
                marker_4036dfc86b8cf480e1a2ac5a0ff2c151.setIcon(icon_51f7f397bb21e6e3670e6646e70b8398);
            
    
                marker_5305a6c366cf3308ce2055fb0717b823.setIcon(icon_794abe103bfe0c3a0d5ae06e70f20356);
            
    
                marker_1474cd1c9ed8151bda8cea4e5c4a4e58.setIcon(icon_a2fa74d8b2ae3c11de4a0f5426bc73d9);
            
    
                marker_5647c956e136169a4359d8a7e9964fb0.setIcon(icon_af768fdb76048a7c525dab7ba7781f00);
            
    
                marker_bf02b94c217e09a3b4b0fe172672f5c6.setIcon(icon_4e2cf668b2e2876154b6787b15e25813);
            
    
            heat_map_db778a2ff2eab7e8f07895f8f3425e77.addTo(map_c8ff09de98adc905a54fc2040c1d5971);
        
    
            tile_layer_d949b83fe6f517e896e0f6c4843cfe36.addTo(map_c8ff09de98adc905a54fc2040c1d5971);
        
    
                marker_3f590acaa38af967496d4a7ce6812e2d.setIcon(icon_dc18ad97906d87525feafb6f7338a80f);
            
    
                marker_a4f037c05a25ab49df8b4d4f8a667c03.setIcon(icon_78b78dec73b94a4b97df30541615ddca);
            
    
                marker_6b26c5a53a2f2faff66663655f121530.setIcon(icon_3b17e3016a68f53730cba3764dab00bd);
            
    
                marker_883bdb94a7a510089568ebdf0d4437ab.setIcon(icon_006e6cc4d6e6d42f911102bb0ae41acc);
            
    
                marker_0a5cd92c6a16602f820d194f95b967e7.setIcon(icon_972bebacfb988009634eca6257aaa943);
            
    
                marker_426697160fc0a77af0ff09c827faea74.setIcon(icon_d5cc3d9a67f425ce3cc7dc5e71bc19e8);
            
    
                marker_43922b55ef8ba27a0f31186a843d91f0.setIcon(icon_f5898716e913f98d632c6069656e1fc9);
            
    
                marker_cd764ee12ad01bb53361441af6fddcc6.setIcon(icon_06292034c9a541eb0c78c8f29ed1b0ee);
            
    
                marker_07e2b95a9383be5b98fc67d2738f4c4c.setIcon(icon_988a57e5383301672753ae8d5b15b2a6);
            
    
                marker_d59f678ad823ae46a2d13dc213f724a1.setIcon(icon_f7ca778969f1c0a7f404222101b8deea);
            
    
                marker_f9e95da173141cba6954fb925ab74b6c.setIcon(icon_8c077bc2b623f9a4a62ec2436ab0a4e1);
            
    
                marker_80e950de2e62359a11fdbcea3f560306.setIcon(icon_6d9f5ade1a4552837272496ce43556e8);
            
    
                marker_86b7bb78898a1126da69cad5fc36fbb9.setIcon(icon_1cdc0b3604a6a407159ba48327427460);
            
    
                marker_d9fcf67510ac995ee8feb7fd1cf0faac.setIcon(icon_5766ef07b6f32f445fa678050bd71b0b);
            
    
                marker_a3197058f827c89bb544c195b110d29d.setIcon(icon_4a423552a90e44a2501136918e3a7477);
            
    
                marker_487022e61230dd5382ed4bd55ff7f856.setIcon(icon_92d62aa9771b073e215117119bc7e0e2);
            
    
                marker_61e71553d595c8fc70c048a78aec7bf7.setIcon(icon_15916f2a36ba01a2468b63988809ec79);
            
    
                marker_cc366cc5c0dbc720e56ba26201d24a70.setIcon(icon_11d1d47a1d40bdfe47983f206d17dcfa);
            
    
                marker_0606b88ee6ce5ceadfd5a41dcf1a23e9.setIcon(icon_cd0ee7bf0fd5ffc72c5b72fd9788a9ee);
            
    
                marker_3a705c43f4dbae8f6189c9f6bd32c09e.setIcon(icon_a626de325cd6302ef1bb1b1b9aa659ab);
            
    
                marker_8dfadf481ecd767e16dd04703e28ec5e.setIcon(icon_480fbe548c59fd152d5d085fc12ac801);
            
    
                marker_3455a3d00352255e1eb471ba0d382ede.setIcon(icon_06c5e247461c3ea62578f6373744df8c);
            
    
                marker_2355a695a3d88d026b841bd22ea0a44e.setIcon(icon_ab833ad763a138f5ee8d96575ea59b46);
            
    
                marker_a3f49352460b89f4fdc394074f42e2e7.setIcon(icon_12e9936a531e94fd5e9d3cee5b4dec1c);
            
    
                marker_523ef938ffb23df9c11e46286bdc2e4b.setIcon(icon_cd9d427f314db9f8c6c08dd476d0340d);
            
    
                marker_885943c0ea96f4a7f6965abe070c72d6.setIcon(icon_c257715adb55c61141bcd5f695f262dc);
            
    
                marker_270e0c6e8a4ea4c23a3579004f5423e5.setIcon(icon_1ea70883537a503a3dd5ec0b66d1aec3);
            
    
                marker_948462a8c8d27a8bead3da64952daa6d.setIcon(icon_8d24760a5a7981e155f8e4a7eb5c47ff);
            
    
                marker_dfeec41f6747008be4aaf1586357d33c.setIcon(icon_5b8961a4f133b510b11981cf7fb3641f);
            
    
                marker_b49f189ced40063eb198ed35de03d024.setIcon(icon_ac0d2c327770a002b45bb22b2692df1f);
            
    
                marker_93313a11aba2910ae2fb886c153a9210.setIcon(icon_42117a88413ed67f06f7432ded10fe69);
            
    
                marker_29130ddb478c66fbdb15d58415791fef.setIcon(icon_2edf867646ac0714c89eed1bb9e52803);
            
    
                marker_6d05676032c49e607aea6663cce5d37c.setIcon(icon_6198fce652fc5ef92a5b6bdb1c3d5d45);
            
    
                marker_19c9d3afb6aad5c11cc7d4a3135cebf0.setIcon(icon_63305b3e13c831cd6e1914782e0bb626);
            
    
                marker_23cd245039ee7571c0efbc63ca0594b2.setIcon(icon_09fb6ad2f21d89a48230b8339a89707f);
            
    
                marker_cd2992d1a1e422de2f7a743aa470deb7.setIcon(icon_18ed817925df8cb5ab575dd4b436f70a);
            
    
                marker_5166b9d2106bd1dfa8a594cc2cdce773.setIcon(icon_6540bdd7aeee829574dc09ecfe8127cd);
            
    
                marker_230e83a44550f779871f328527e1a7c6.setIcon(icon_d71140e589b0008f193280746f88c767);
            
    
                marker_44700b15946f2c45142a56b3b58b2f7b.setIcon(icon_440cc7e3da7eb5dea4859dbe127a308a);
            
    
                marker_d440f326e39957b309d2ecfe725fa50a.setIcon(icon_6f7b3be33ea4d0f6cec4015bfece332d);
            
    
                marker_9280a5f457be8c5faaae181efe1f406e.setIcon(icon_f0ccee8d31a39d9fd01ba658bc72ef94);
            
    
                marker_571a1a42b8f1dc2a2990a5613b94d545.setIcon(icon_838798fa0a21290874c30c35228b4fcf);
            
    
                marker_52e09b4f2ab34c4526a772e2f22aaaab.setIcon(icon_72c9807d85b0fa2f1b7b4d4f36281862);
            
    
                marker_1a373d2474965bba0ebd9dfc59f82625.setIcon(icon_435f95e3e167d1e74d94a1679b2d5404);
            
    
                marker_96c9381721b8cdfb9ec02c447577ec79.setIcon(icon_d06070aea1b38ebd363510d20e146800);
            
    
                marker_7d82b8e756fec4f491a6bdbbfe5f0b68.setIcon(icon_c7b05e6bb23107e3b575a5ba81b6c622);
            
    
                marker_0ca06a8a9a77cde85e964e44ac38cca5.setIcon(icon_b4d04f32c7c36e95251f65a957b1ea71);
            
    
                marker_6a70d51d00aa17fd1428fe6126711c65.setIcon(icon_c44be28ae9969a9e620e2f09efbf630f);
            
    
                marker_111987d43e2e7d0ef1ad3f190b1a8d60.setIcon(icon_24487bc7c70da498ad3565edad11d1e1);
            
    
                marker_832e5a8df64b158fcae2284f69ad00af.setIcon(icon_23c9dcd84d1086bdeff00907efdcb9ca);
            
    
                marker_f000f0b2f2f850268faccb1a26738a2a.setIcon(icon_966ad09b0dfcfdaa5a0842da70a331ac);
            
    
                marker_58cbe95711a9b5d33ba4744c94919eea.setIcon(icon_9b2814a157a58b4b1e7a54de599625a1);
            
    
                marker_8be7e6c3da0f62cb2b554ff26d421088.setIcon(icon_64d0e49bf5a3fe38c19b879a31dc15f8);
            
    
                marker_0a42340b37b71bec5ecc9c7b522a8114.setIcon(icon_ddd8bf1aacd6af0b11435de717def930);
            
    
                marker_04410cfb1fd03a9687fdb67aa107ac0a.setIcon(icon_a6e9326734b73fe90b4b8ba95e22fb68);
            
    
                marker_026790a28da075b50ed66d0317c22a48.setIcon(icon_4f67843e2a48729be6e8dde9e2f85186);
            
    
                marker_c89d1548a3acbb850f7cea7e71b316fe.setIcon(icon_769c1c0a13fdf8623b213e57b0611752);
            
    
                marker_3402447f031eb12dc69a14395dcb04df.setIcon(icon_0f7a58fdb08b510f6aa186da5355b22f);
            
    
                marker_37a9e816cbe54ad4458f989295bb4a4d.setIcon(icon_44b27971918149696bb29828de1519e6);
            
    
                marker_80b52283ba24af338208ac1649e28d49.setIcon(icon_076db85b550048fb937fde4fc9946b93);
            
    
                marker_a3a304dfcb376c3afc464ed1b31677fc.setIcon(icon_fe3c3f1442d2f2e90157a82e333e00fa);
            
    
                marker_ee81207fe12c33b1ffbae49b5f76bbf6.setIcon(icon_6e58629d83dab2366f208a31e5e76f47);
            
    
                marker_4fa223fd0f691b4b122c33c4aa0ec047.setIcon(icon_7a73e2d7c4eb76a18cd56995d68133cc);
            
    
                marker_972ecab2d5cf5031f6b09ad532b34835.setIcon(icon_8a63ed2bb38d1f03ed32459b7c55b21a);
            
    
                marker_f8bdb4bcf77e304c69bc1ae87ce2b28d.setIcon(icon_83085ce02c34423f7e2a81a8e4a35785);
            
    
                marker_68377d78b2f8030063487a22217262d3.setIcon(icon_0ccfa41473ba50569d31a133ab3c291e);
            
    
                marker_35b1baf669cb5a32c092567b9699ad15.setIcon(icon_2a0f0a57a85f7c68bf866141be463574);
            
    
                marker_2006d49cbef7b9eec684a9b222550d7b.setIcon(icon_d631429be6e03f682419616c192b37f6);
            
    
                marker_2f1b99b156b9dc3cd7be1eec10d2eec2.setIcon(icon_cc9ab042445a62eed1c7884a97620536);
            
    
                marker_edecf5ed21156bd7b6e3e04ab96bb1e7.setIcon(icon_97ed0db7e862c1649a88178eb0c19b0c);
            
    
                marker_fe9f7d01595836dabfe5852f06f58873.setIcon(icon_9bd793c1cabf4394dee9f4e972999b90);
            
    
                marker_34fedc988d54a1fb1ae610661c007dc2.setIcon(icon_7e11d665dc56962cd509799d493c67a3);
            
    
                marker_36126a261aae9eb1b55847a5422a148b.setIcon(icon_9b180d7a045a8c3f8a2ac814a4ce402b);
            
    
                marker_f5e5f7df69dbf1aee32bab61e655b166.setIcon(icon_a1a8a41706ce4de5159fa120186079b9);
            
    
                marker_5e6a671374464638c603f1562926bf4f.setIcon(icon_26c18767f238c9693b636274491ace6b);
            
    
                marker_b6090a01162ad3b1c61e5dc8710f32e8.setIcon(icon_cad434cec9f23721e65896ad9e26132e);
            
    
                marker_1dc43eab709063b970ccb25f27aa8a61.setIcon(icon_d3d85b21bf5d48c72bb835089ab921a7);
            
    
                marker_8b843c7b7882ae31e15d0cc0ab9a8e92.setIcon(icon_d4df04fe19e5898d5a6deb910924989c);
            
    
                marker_cfa12262e38d5a4b670f38162aae5c14.setIcon(icon_f78195e4e5acc8e39a9cd1bb67b53f05);
            
    
                marker_337b69dda4af2166ce6c1aec5fed529c.setIcon(icon_bf6bce2f5d9c98c515b0f1c387e288e0);
            
    
                marker_6788e17e1cfd2b794853866f52ed822a.setIcon(icon_861c30eeeb95fdae83148d1b636306f8);
            
    
                marker_3a535b0c2787cd5d7fdf80d412f4bd16.setIcon(icon_055c6f95e2625ed41f137d5287c4e3c4);
            
    
                marker_b2cbf593196a58236bfe392270b5c87e.setIcon(icon_3cf91eba70c4769f9f388968dd06788c);
            
    
                marker_0111f9504e523a0cb15ae333ee53c051.setIcon(icon_e70368ee1aa02912855ec1ec238adc45);
            
    
                marker_6c143d9b2d0681a578cec5d3358d7a47.setIcon(icon_f9b6dae57e9cc94f446ce6a909c9fa16);
            
    
                marker_4036dfc86b8cf480e1a2ac5a0ff2c151.setIcon(icon_51f7f397bb21e6e3670e6646e70b8398);
            
    
                marker_5305a6c366cf3308ce2055fb0717b823.setIcon(icon_794abe103bfe0c3a0d5ae06e70f20356);
            
    
                marker_1474cd1c9ed8151bda8cea4e5c4a4e58.setIcon(icon_a2fa74d8b2ae3c11de4a0f5426bc73d9);
            
    
                marker_5647c956e136169a4359d8a7e9964fb0.setIcon(icon_af768fdb76048a7c525dab7ba7781f00);
            
    
                marker_bf02b94c217e09a3b4b0fe172672f5c6.setIcon(icon_4e2cf668b2e2876154b6787b15e25813);
            
    
            heat_map_db778a2ff2eab7e8f07895f8f3425e77.addTo(map_c8ff09de98adc905a54fc2040c1d5971);
        
</script>
</html>
