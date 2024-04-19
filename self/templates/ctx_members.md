{{#membersOrd}}
1. **{{#body.title}}{{.}}{{/body.title}}**{{^body.title}}*untitled*{{/body.title}} ({{body.entity_title}}) :id: [{{id}}](/entities/seaf.self/object_card?id={{id}}) {{#body.exposed}}:arrow_right: [{{augments}}](/entities/seaf.self/object_card?id={{augments}}) {{/body.exposed}} {{#body.impressed}}{{^body.overriden}}:warning:{{/body.overriden}}:arrow_left: [{{.}}](/entities/seaf.self/object_card?id={{.}}) {{/body.impressed}}
{{/membersOrd}}
{{#membersCtx}}
1. **{{#body.title}}{{.}}{{/body.title}}**{{^body.title}}*untitled*{{/body.title}} ({{body.entity_title}}) :id: [{{id}}](/entities/seaf.self/object_card?id={{id}}) :arrow_down: [drilldown](/entities/seaf.self/ctx_summary?domain={{id}}) {{#body.exposed}}:arrow_right: [{{augments}}](/entities/seaf.self/object_card?id={{augments}}) {{/body.exposed}} {{#body.impressed}}{{^body.overriden}}:warning:{{/body.overriden}}:arrow_left: {{.}} {{/body.impressed}}
{{/membersCtx}}
