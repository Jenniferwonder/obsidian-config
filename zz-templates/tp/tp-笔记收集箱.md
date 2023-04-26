<%-*  let filetype = await tp.system.suggester(["Resource","Project","Tracking","Temp"], ["Resource","Project","Tracking","Temp"], false, "Which template do you want to use?") -%>
<%-* if (filetype === "Resource") {  -%>
<%-tp.file.include("[[tp-资源分类模板]]")-%>
<%-* } else if (filetype === "Project") {  -%>
<%-tp.file.include("[[tp-流水账模板]]")-%>
<%-* } else if (filetype === "Tracking") {  -%>
<%-tp.file.include("[[tp-人物模板]]")-%>
<%-* } else if (filetype === "Temp") {  -%>
<%-tp.file.include("[[zz-templates/tp/tp-通用模板]]")-%>
<%-* } else { -%>
<%-tp.file.include("[[zz-templates/tp/tp-通用模板]]")-%>
<%-* } -%>