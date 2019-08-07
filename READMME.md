# Estudos em delphi
```PASCAL
  try
    RESTRequest1.Resource := 'ws/{CEP}/json/';
    RESTRequest1.Params.AddUrlSegment('CEP', edtCEP.Text);
    RESTRequest1.Execute;
    aRetorno := RESTRequest1.Response.JSONValue as TJSONObject;
  except on e:Exception do
    begin
      ShowMessage('Erro no WebService tente mais tarde!');
      raise;
    end;
  end;```
  
  Gladson eu mexi nesta rotina e nao sei porque pariu de funcionar.
