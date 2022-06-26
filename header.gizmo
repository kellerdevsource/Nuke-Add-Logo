#! C:/Program Files/Nuke11.3v4/nuke-11.3.4.dll -nx
version 11.3 v4
Gizmo {
 addUserKnob {20 User}
 addUserKnob {1 comment t comment}
 comment Section_GEMUE_650_zu
 addUserKnob {1 project l Project}
 project "Test Project"
 addUserKnob {1 version l Version}
 version v1
 addUserKnob {22 set l Set T "group = nuke.thisNode()\nwith group:\n    nuke.toNode(\"Text1\").knob(\"message\").setValue(nuke.thisNode().knob(\"project\").value())\n    nuke.toNode(\"Text3\").knob(\"message\").setValue(nuke.thisNode().knob(\"version\").value())\n    nuke.toNode(\"Text4\").knob(\"message\").setValue(nuke.thisNode().knob(\"comment\").value())" +STARTLINE}
}
 Read {
  inputs 0
  file_type png
  file "White.png"
  origset true
  in_colorspace linear
  out_colorspace linear
  name Read1
  xpos -133
  ypos 161
 }
 Premult {
  name Premult1
  xpos -133
  ypos 278
 }
 Transform {
  translate {{"\[python nuke.toNode(\\\"Rectangle1\\\").input(0).width()/100]"} {"\[python nuke.toNode(\\\"Rectangle1\\\").input(0).height()/150]"}}
  scale {{"\[python nuke.toNode(\\\"Rectangle1\\\").input(0).height()/41000]"}}
  name Transform1
  xpos -133
  ypos 320
 }
 Input {
  inputs 0
  name Input1
  xpos 0
 }
 Rectangle {
  opacity 0.9
  area {0 0 {"\[python nuke.thisNode().input(0).width()]"} {"\[python nuke.thisNode().input(0).height()/20]"}}
  color 0
  name Rectangle1
  selected true
  xpos 0
  ypos 73
 }
 Rectangle {
  opacity 0.9
  area {0 {"\[python nuke.thisNode().input(0).height()-nuke.thisNode().input(0).height()/20]"} {"\[python nuke.thisNode().input(0).width()]"} {"\[python nuke.thisNode().input(0).height()]"}}
  color 0
  name Rectangle2
  selected true
  xpos 0
  ypos 108
 }
 Text {
  message "Test Project"
  font C:/Windows/Fonts/consola.ttf
  size {{"\[python nuke.thisNode().input(0).height()/55]"}}
  yjustify center
  Transform 1
  box {{"\[python nuke.thisNode().input(0).width()/100]"} {"\[python nuke.thisNode().input(0).height()-nuke.thisNode().input(0).height()/20]"} {"\[python nuke.thisNode().input(0).width()/2]"} {"\[python nuke.thisNode().input(0).height()]"}}
  center {{"\[python nuke.thisNode().input(0).width()/2]"} {"\[python nuke.thisNode().input(0).height()/2]"}}
  name Text1
  xpos 0
  ypos 150
 }
 Text {
  message "\[date %x]"
  font C:/Windows/Fonts/consola.ttf
  size {{"\[python nuke.thisNode().input(0).height()/55]"}}
  xjustify center
  yjustify center
  Transform 1
  box {{"\[python nuke.thisNode().input(0).width()-nuke.thisNode().input(0).width()*15/100]"} 0 {"\[python nuke.thisNode().input(0).width()-nuke.thisNode().input(0).width()/100]"} {"\[python nuke.thisNode().input(0).height()/20]"}}
  center {{"\[python nuke.thisNode().input(0).width()/2]"} {"\[python nuke.thisNode().input(0).height()/2]"}}
  name Text2
  xpos 0
  ypos 182
 }
 Text {
  message v1
  font C:/Windows/Fonts/consola.ttf
  size {{"\[python nuke.thisNode().input(0).height()/55]"}}
  xjustify center
  yjustify center
  Transform 1
  box {{"\[python nuke.thisNode().input(0).width()-nuke.thisNode().input(0).width()*25/100]"} 0 {"\[python nuke.thisNode().input(0).width()-nuke.thisNode().input(0).width()*15/100]"} {"\[python nuke.thisNode().input(0).height()/20]"}}
  center {{"\[python nuke.thisNode().input(0).width()/2]"} {"\[python nuke.thisNode().input(0).height()/2]"}}
  name Text3
  xpos 0
  ypos 213
  addUserKnob {20 User}
 }
 Text {
  message Section_GEMUE_650_zu
  font C:/Windows/Fonts/consola.ttf
  size {{"\[python nuke.thisNode().input(0).height()/55]"}}
  xjustify right
  yjustify center
  Transform 1
  box {{"\[python nuke.thisNode().input(0).width()-nuke.thisNode().input(0).width()*70/100]"} 0 {"\[python nuke.thisNode().input(0).width()-nuke.thisNode().input(0).width()*25/100]"} {"\[python nuke.thisNode().input(0).height()/20]"}}
  center {{"\[python nuke.thisNode().input(0).width()/2]"} {"\[python nuke.thisNode().input(0).height()/2]"}}
  name Text4
  xpos 0
  ypos 247
  addUserKnob {20 User}
 }
 Merge {
  inputs 2
  name Merge1
  xpos 0
  ypos 320
 }
 Output {
  name Output1
  xpos 0
  ypos 381
 }
 Viewer {
  frame_range 1-100
  name Viewer1
  xpos 100
  ypos 489
 }
end_group
