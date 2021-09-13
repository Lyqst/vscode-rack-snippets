# vcv-rack-snippets

Visual Studio Code snippets for VCV Rack module development .

## Snippet list

### Module

|Prefix|Code|
|-|-|
|```!module```|Full module boilerplate code|
|```!config```|```configParam(${1:param}, ${2:minvalue}, ${3:maxvalue}, ${4:defaultvalue}, "${5:label}");```|
|```!json```|```json_t *dataToJson() override {} void dataFromJson(json_t *rootJ) override {}```|

### Input

|Prefix|Code|
|-|-|
|```!igetvoltage```|```inputs[${1:input}].getVoltage($2);```|
|```!igetvoltages```|```inputs[${1:input}].getVoltages($2);```|
|```!igetchannels```|```inputs[${1:input}].getChannels();```|

### Params

|Prefix|Code|
|-|-|
|```!pgetvalue```|```params[${1:param}].getValue();```|
|```!psetvalue```|```params[${1:param}].setValue($2);```|

### Output

|Prefix|Code|
|-|-|
|```!osetvoltage```|```outputs[${1:output}].setVoltage($2, $3);```|
|```!ogetchannels```|```outputs[${1:output}].setChannels($2);```|

### Widget

|Prefix|Code|
|-|-|
|```!winput```|```addInput(createInputCentered<${1:widget}>(Vec($2, $3), module, ${4:input}));```|
|```!wparam```|```addParam(createParamCentered<${1:widget}>(Vec($2, $3), module, ${4:param}));```|
|```!woutput```|```addOutput(createOutCentered<${1:widget}>(Vec($2, $3), module, ${4:output}));```|
|```!widget```|```addChild(createWidget<${1:widget}>(Vec(Vec($2, $3)));```|

### Plugin

|Prefix|Code|
|-|-|
|```!addmodel```|```p->addModel(model${1:slug});```|
|```!externmodel```|```extern Model* model${1:slug};```|
|```!info```|"Slug", "name", "description" and "tags" in json format for plugin.json|