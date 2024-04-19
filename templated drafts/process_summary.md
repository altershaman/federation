###### :id: {{id}}
---
{{^process_error}}
:warning: Такого объекта не существует
{{/process_error}}

{{#process_error}}
# Участник: "{{body.title}}" 
{{body.description}}

###### входит в контекст {{#wrapper.body.title}}"{{.}}"{{/wrapper.body.title}}{{^wrapper.body.title}}"Глобальный"{{/wrapper.body.title}} :id:{{#wrapper.id}}{{.}}{{/wrapper.id}}{{^wrapper.id}}ctxG{{/wrapper.id}}:

{{#neighboursCtx}}
* {{body.title}} (контекст)
{{/neighboursCtx}}
{{#neighboursOrd}}
* {{body.title}}
{{/neighboursOrd}}

###### {{#isContext}}является контекстом для:

{{#membersCtx}}
* **{{#body.title}}{{.}}{{/body.title}}{{^body.title}}untitled{{/body.title}}** (контекст) :id: {{id}}
    {{#body.impressed}}* Фасад: {{.}}{{/body.impressed}}
{{/membersCtx}}
{{#membersOrd}}
* **{{#body.title}}{{.}}{{/body.title}}{{^body.title}}untitled{{/body.title}}** :id: {{id}}
    {{#body.impressed}}* фасад: {{.}}{{/body.impressed}}
{{/membersOrd}}

{{/isContext}}

{{/process_error}}