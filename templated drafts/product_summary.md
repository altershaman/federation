###### :id: {{id}}
---
{{^product_error}}
:warning: Такого объекта не существует
{{/product_error}}

{{#product_error}}
# Продукт: "{{body.title}}" 
{{body.description}}

###### входит в контекст {{#wrapper.body.title}}"{{.}}"{{/wrapper.body.title}}{{^wrapper.body.title}}"Глобальный"{{/wrapper.body.title}} :id:{{#wrapper.id}}{{.}}{{/wrapper.id}}{{^wrapper.id}}ctxG{{/wrapper.id}}:

{{#neighboursCtx}}
* {{body.title}} (контекст) :id: [{{id}}](/entities/{{body.entity_id}}/ctx_summary?domain={{id}})
{{/neighboursCtx}}
{{#neighboursOrd}}
* {{body.title}} :id: [{{id}}](/entities/{{body.entity_id}}/ctx_summary?domain={{id}})
{{/neighboursOrd}}

###### {{#isContext}}является контекстом для:

{{#membersCtx}}
* **{{#body.title}}{{.}}{{/body.title}}{{^body.title}}untitled{{/body.title}}** (контекст) :id: [{{id}}](/entities/{{body.entity_id}}/ctx_summary?domain={{id}})
    {{#body.impressed}}* Фасад: {{.}}{{/body.impressed}}
{{/membersCtx}}
{{#membersOrd}}
* **{{#body.title}}{{.}}{{/body.title}}{{^body.title}}untitled{{/body.title}}** :id: [{{id}}](/entities/{{body.entity_id}}/ctx_summary?domain={{id}})
    {{#body.impressed}}* фасад: {{.}}{{/body.impressed}}
{{/membersOrd}}

{{/isContext}}

{{/product_error}}