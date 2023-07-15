<%-*  let filetype = await tp.system.suggester(["Resource","Project","Tracking","Temp"], ["Resource","Project","Tracking","Temp"], false, "Which template do you want to use?") -%>
<%-* if (filetype === "Resource") {  -%>
<%-tp.file.include("[[tp-资源分类模板]]")-%>
<%-* } else if (filetype === "Project") {  -%>
<%-tp.file.include("[[tp-Tasks]]")-%>
<%-* } else if (filetype === "Tracking") {  -%>
<%-tp.file.include("[[tp-人物模板]]")-%>
<%-* } else if (filetype === "Temp") {  -%>
<%-tp.file.include("[[tp-GNotes]]")-%>
<%-* } else { -%>
<%-tp.file.include("[[tp-GNotes]]")-%>
<%-* } -%>