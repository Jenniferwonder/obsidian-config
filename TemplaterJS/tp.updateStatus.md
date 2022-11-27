<%*
const file = tp.file.find_tfile(tp.file.title);
const {update} = app.plugins.plugins["metaedit"].api;
const status = tp.frontmatter.status;
if (status === "Doing") {
 await update("status","Done",file);
}
if (status === "Todo") {
await update("status", "Doing", file);
}
if (status === "Done") {
await update("status", "Todo", file);
}
-%>