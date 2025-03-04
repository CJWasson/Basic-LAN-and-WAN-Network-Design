<mxfile host="app.diagrams.net" agent="Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/133.0.0.0 Safari/537.36" version="26.0.15">
  <diagram name="Home Network Diagram" id="0">
    <mxGraphModel dx="2805" dy="1749" grid="1" gridSize="10" guides="1" tooltips="1" connect="1" arrows="1" fold="1" page="1" pageScale="1" pageWidth="827" pageHeight="1169" math="0" shadow="0">
      <root>
        <mxCell id="0" />
        <mxCell id="1" parent="0" />
        <mxCell id="2" value="Internet" style="ellipse;fillColor=#D4E157;strokeColor=#000000" parent="1" vertex="1">
          <mxGeometry x="400" y="50" width="100" height="50" as="geometry" />
        </mxCell>
        <mxCell id="3" value="Firewall" style="shape=hexagon;fillColor=#FF7043;strokeColor=#000000" parent="1" vertex="1">
          <mxGeometry x="400" y="120" width="100" height="50" as="geometry" />
        </mxCell>
        <mxCell id="4" parent="1" source="2" target="3" edge="1" />
        <mxCell id="5" value="Router" style="shape=trapezoid;fillColor=#64B5F6;strokeColor=#000000" parent="1" vertex="1">
          <mxGeometry x="400" y="190" width="100" height="50" as="geometry" />
        </mxCell>
        <mxCell id="6" parent="1" source="3" target="5" edge="1" />
        <mxCell id="7" value="Switch" style="shape=rectangle;fillColor=#FFEB3B;strokeColor=#000000" parent="1" vertex="1">
          <mxGeometry x="400" y="260" width="100" height="50" as="geometry" />
        </mxCell>
        <mxCell id="8" parent="1" source="5" target="7" edge="1" />
        <mxCell id="9" value="Wireless AP" style="shape=ellipse;fillColor=#81C784;strokeColor=#000000" parent="1" vertex="1">
          <mxGeometry x="550" y="260" width="100" height="50" as="geometry" />
        </mxCell>
        <mxCell id="10" parent="1" source="5" target="9" edge="1" />
        <mxCell id="11" value="PC 1" style="shape=rectangle;fillColor=#90CAF9;strokeColor=#000000" parent="1" vertex="1">
          <mxGeometry x="300" y="330" width="100" height="50" as="geometry" />
        </mxCell>
        <mxCell id="12" parent="1" source="7" target="11" edge="1" />
        <mxCell id="13" value="PC 2" style="shape=rectangle;fillColor=#90CAF9;strokeColor=#000000" parent="1" vertex="1">
          <mxGeometry x="400" y="330" width="100" height="50" as="geometry" />
        </mxCell>
        <mxCell id="14" parent="1" source="7" target="13" edge="1" />
        <mxCell id="15" value="Laptop" style="shape=rectangle;fillColor=#90CAF9;strokeColor=#000000" parent="1" vertex="1">
          <mxGeometry x="550" y="330" width="100" height="50" as="geometry" />
        </mxCell>
        <mxCell id="16" parent="1" source="9" target="15" edge="1" />
        <mxCell id="17" value="Printer" style="shape=rectangle;fillColor=#A5D6A7;strokeColor=#000000" parent="1" vertex="1">
          <mxGeometry x="200" y="330" width="100" height="50" as="geometry" />
        </mxCell>
        <mxCell id="18" parent="1" source="7" target="17" edge="1" />
        <mxCell id="KHUMOH-2GiU43_IcQN2v-18" value="Internet" style="ellipse;fillColor=#D4E157;strokeColor=#000000" vertex="1" parent="1">
          <mxGeometry x="400" y="50" width="100" height="50" as="geometry" />
        </mxCell>
        <mxCell id="KHUMOH-2GiU43_IcQN2v-19" value="Firewall" style="shape=hexagon;fillColor=#FF7043;strokeColor=#000000" vertex="1" parent="1">
          <mxGeometry x="400" y="120" width="100" height="50" as="geometry" />
        </mxCell>
        <mxCell id="KHUMOH-2GiU43_IcQN2v-20" edge="1" parent="1" source="KHUMOH-2GiU43_IcQN2v-18" target="KHUMOH-2GiU43_IcQN2v-19" />
        <mxCell id="KHUMOH-2GiU43_IcQN2v-21" value="Router" style="shape=trapezoid;fillColor=#64B5F6;strokeColor=#000000" vertex="1" parent="1">
          <mxGeometry x="400" y="190" width="100" height="50" as="geometry" />
        </mxCell>
        <mxCell id="KHUMOH-2GiU43_IcQN2v-22" edge="1" parent="1" source="KHUMOH-2GiU43_IcQN2v-19" target="KHUMOH-2GiU43_IcQN2v-21" />
        <mxCell id="KHUMOH-2GiU43_IcQN2v-23" value="Switch" style="shape=rectangle;fillColor=#FFEB3B;strokeColor=#000000" vertex="1" parent="1">
          <mxGeometry x="400" y="260" width="100" height="50" as="geometry" />
        </mxCell>
        <mxCell id="KHUMOH-2GiU43_IcQN2v-24" edge="1" parent="1" source="KHUMOH-2GiU43_IcQN2v-21" target="KHUMOH-2GiU43_IcQN2v-23" />
        <mxCell id="KHUMOH-2GiU43_IcQN2v-25" value="Wireless AP" style="shape=ellipse;fillColor=#81C784;strokeColor=#000000" vertex="1" parent="1">
          <mxGeometry x="550" y="260" width="100" height="50" as="geometry" />
        </mxCell>
        <mxCell id="KHUMOH-2GiU43_IcQN2v-26" edge="1" parent="1" source="KHUMOH-2GiU43_IcQN2v-21" target="KHUMOH-2GiU43_IcQN2v-25" />
        <mxCell id="KHUMOH-2GiU43_IcQN2v-27" value="PC 1" style="shape=rectangle;fillColor=#90CAF9;strokeColor=#000000" vertex="1" parent="1">
          <mxGeometry x="300" y="330" width="100" height="50" as="geometry" />
        </mxCell>
        <mxCell id="KHUMOH-2GiU43_IcQN2v-28" edge="1" parent="1" source="KHUMOH-2GiU43_IcQN2v-23" target="KHUMOH-2GiU43_IcQN2v-27" />
        <mxCell id="KHUMOH-2GiU43_IcQN2v-29" value="PC 2" style="shape=rectangle;fillColor=#90CAF9;strokeColor=#000000" vertex="1" parent="1">
          <mxGeometry x="400" y="330" width="100" height="50" as="geometry" />
        </mxCell>
        <mxCell id="KHUMOH-2GiU43_IcQN2v-30" edge="1" parent="1" source="KHUMOH-2GiU43_IcQN2v-23" target="KHUMOH-2GiU43_IcQN2v-29" />
        <mxCell id="KHUMOH-2GiU43_IcQN2v-31" value="Laptop" style="shape=rectangle;fillColor=#90CAF9;strokeColor=#000000" vertex="1" parent="1">
          <mxGeometry x="550" y="330" width="100" height="50" as="geometry" />
        </mxCell>
        <mxCell id="KHUMOH-2GiU43_IcQN2v-32" edge="1" parent="1" source="KHUMOH-2GiU43_IcQN2v-25" target="KHUMOH-2GiU43_IcQN2v-31" />
        <mxCell id="KHUMOH-2GiU43_IcQN2v-33" value="Printer" style="shape=rectangle;fillColor=#A5D6A7;strokeColor=#000000" vertex="1" parent="1">
          <mxGeometry x="200" y="330" width="100" height="50" as="geometry" />
        </mxCell>
        <mxCell id="KHUMOH-2GiU43_IcQN2v-34" edge="1" parent="1" source="KHUMOH-2GiU43_IcQN2v-23" target="KHUMOH-2GiU43_IcQN2v-33" />
        <mxCell id="KHUMOH-2GiU43_IcQN2v-35" value="Internet" style="ellipse;fillColor=#D4E157;strokeColor=#000000" vertex="1" parent="1">
          <mxGeometry x="400" y="50" width="100" height="50" as="geometry" />
        </mxCell>
        <mxCell id="KHUMOH-2GiU43_IcQN2v-36" value="Firewall" style="shape=hexagon;fillColor=#FF7043;strokeColor=#000000" vertex="1" parent="1">
          <mxGeometry x="400" y="120" width="100" height="50" as="geometry" />
        </mxCell>
        <mxCell id="KHUMOH-2GiU43_IcQN2v-37" edge="1" parent="1" source="KHUMOH-2GiU43_IcQN2v-35" target="KHUMOH-2GiU43_IcQN2v-36" />
        <mxCell id="KHUMOH-2GiU43_IcQN2v-38" value="Router" style="shape=trapezoid;fillColor=#64B5F6;strokeColor=#000000" vertex="1" parent="1">
          <mxGeometry x="400" y="190" width="100" height="50" as="geometry" />
        </mxCell>
        <mxCell id="KHUMOH-2GiU43_IcQN2v-39" edge="1" parent="1" source="KHUMOH-2GiU43_IcQN2v-36" target="KHUMOH-2GiU43_IcQN2v-38" />
        <mxCell id="KHUMOH-2GiU43_IcQN2v-40" value="Switch" style="shape=rectangle;fillColor=#FFEB3B;strokeColor=#000000" vertex="1" parent="1">
          <mxGeometry x="400" y="260" width="100" height="50" as="geometry" />
        </mxCell>
        <mxCell id="KHUMOH-2GiU43_IcQN2v-41" edge="1" parent="1" source="KHUMOH-2GiU43_IcQN2v-38" target="KHUMOH-2GiU43_IcQN2v-40" />
        <mxCell id="KHUMOH-2GiU43_IcQN2v-42" value="Wireless AP" style="shape=ellipse;fillColor=#81C784;strokeColor=#000000" vertex="1" parent="1">
          <mxGeometry x="550" y="260" width="100" height="50" as="geometry" />
        </mxCell>
        <mxCell id="KHUMOH-2GiU43_IcQN2v-43" edge="1" parent="1" source="KHUMOH-2GiU43_IcQN2v-38" target="KHUMOH-2GiU43_IcQN2v-42" />
        <mxCell id="KHUMOH-2GiU43_IcQN2v-44" value="PC 1" style="shape=rectangle;fillColor=#90CAF9;strokeColor=#000000" vertex="1" parent="1">
          <mxGeometry x="300" y="330" width="100" height="50" as="geometry" />
        </mxCell>
        <mxCell id="KHUMOH-2GiU43_IcQN2v-45" edge="1" parent="1" source="KHUMOH-2GiU43_IcQN2v-40" target="KHUMOH-2GiU43_IcQN2v-44" />
        <mxCell id="KHUMOH-2GiU43_IcQN2v-46" value="PC 2" style="shape=rectangle;fillColor=#90CAF9;strokeColor=#000000" vertex="1" parent="1">
          <mxGeometry x="400" y="330" width="100" height="50" as="geometry" />
        </mxCell>
        <mxCell id="KHUMOH-2GiU43_IcQN2v-47" edge="1" parent="1" source="KHUMOH-2GiU43_IcQN2v-40" target="KHUMOH-2GiU43_IcQN2v-46" />
        <mxCell id="KHUMOH-2GiU43_IcQN2v-48" value="Laptop" style="shape=rectangle;fillColor=#90CAF9;strokeColor=#000000" vertex="1" parent="1">
          <mxGeometry x="550" y="330" width="100" height="50" as="geometry" />
        </mxCell>
        <mxCell id="KHUMOH-2GiU43_IcQN2v-49" edge="1" parent="1" source="KHUMOH-2GiU43_IcQN2v-42" target="KHUMOH-2GiU43_IcQN2v-48" />
        <mxCell id="KHUMOH-2GiU43_IcQN2v-50" value="Printer" style="shape=rectangle;fillColor=#A5D6A7;strokeColor=#000000" vertex="1" parent="1">
          <mxGeometry x="200" y="330" width="100" height="50" as="geometry" />
        </mxCell>
        <mxCell id="KHUMOH-2GiU43_IcQN2v-51" edge="1" parent="1" source="KHUMOH-2GiU43_IcQN2v-40" target="KHUMOH-2GiU43_IcQN2v-50" />
      </root>
    </mxGraphModel>
  </diagram>
</mxfile>
