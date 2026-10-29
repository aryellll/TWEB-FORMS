# TWEB-FORMS
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Inscrição nos jogos escolares</title>
</head>
<body>
   <header>
    
    <h1>Inscrição nos jogos escolares</h1>
    Preencha os campos com suas informações.
   </header>
   
        <main>
        <form id="inscrição-jogos" action="inscrições-jogos" method="post" enctype="multipart/form-data">
        
        <fieldset>
        <legend>Identificação do atleta</legend>
        <label for="nome-atleta">Nome completo do atleta (obrigatório)</label>
        <input type="text" id="nome-atleta" name="nome-atleta" required>

        <label for="email-atleta">E-mail de contato (obrigatório)</label>
        <input type="email" id="email-atleta" name="email-atleta" required>
        </fieldset>

        <fieldset>
        <legend>Participação nos jogos</legend>
        <label for="equipe">Nome da equipe</label>
        <input type="text" id="equipe" name="equipe" value="Equipe Horizonte">

        <fieldset>
        <legend>Turno de preferência</legend>
        <input type="radio" id="turno-manha" name="turno" value="manha">
        <label for="turno-manha">Manhã</label>
        <input type="radio" id="turno-tarde" name="turno" value="tarde">
        <label for="turno-tarde">Tarde</label>
        <fieldset>
        <legend>Modalidades de interesse</legend>
        <input type="checkbox" id="interesse-futsal"
name="modalidades" value="futsal">
        <label for="interesse-futsal">Futsal</label>
        <input type="checkbox" id="interesse-volei"
name="modalidades" value="voleibol">
        <label for="interesse-volei">Voleibol</label>
        <label for="modalidade-principal">Modalidade principal (obrigatória)</label>
        <select id="modalidade-principal" name="modalidade_principal" required>
        <option value="">Selecione uma modalidade</option>
        <optgroup label="Coletivas">
        <option value="futsal">Futsal</option>
        <option value="voleibol">Voleibol</option>
        </optgroup>
        <optgroup label="Individuais">
        <option value="atletismo">Atletismo</option>
        <option value="xadrez">Xadrez</option>
        </optgroup>
        </select>
        <label for="escola">Escola de origem</label>
        <input type="search" id="escola" name="escola" list="escolas">
        <datalist id="escolas">
        <option value="Escola Horizonte"></option>
        <option value="Escola Aurora"></option>
        <option value="Escola Caminhos"></option>
        </datalist>
        <label for="observacoes">Observações para a organização</label>
        <textarea id="observacoes" name="observacoes" rows="5" cols="50"></textarea>
        <textarea id="recado" name="recado" rows="3" cols="50">Participarei da abertura.</textarea>
        <button type="submit" name="acao" value="inscrever">Confirmar inscrição</button>
</fieldset>
    
    
    </form>

    
   </main>
</body>
</html>
