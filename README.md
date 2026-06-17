<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <script src="https://cdn.tailwindcss.com"></script>
</head>
<body class="bg-slate-950 text-slate-200 p-8">
    <div class="grid grid-cols-1 md:grid-cols-4 gap-4 mb-8">
        <div class="bg-slate-900 p-6 rounded-2xl border border-slate-800">
            <h3 class="text-slate-500 text-xs uppercase font-bold">Taxa de Conversão</h3>
            <p class="text-3xl font-black text-emerald-400">14.2%</p>
        </div>
        <div class="bg-slate-900 p-6 rounded-2xl border border-slate-800">
            <h3 class="text-slate-500 text-xs uppercase font-bold">Pipeline Valor (Estimado)</h3>
            <p class="text-3xl font-black text-blue-400">R$ 179.800</p>
        </div>
        <div class="bg-slate-900 p-6 rounded-2xl border border-slate-800">
            <h3 class="text-slate-500 text-xs uppercase font-bold">Leads Ativos</h3>
            <p class="text-3xl font-black text-white">45</p>
        </div>
        <div class="bg-slate-900 p-6 rounded-2xl border border-slate-800">
            <h3 class="text-slate-500 text-xs uppercase font-bold">Velocidade (Lead/Dia)</h3>
            <p class="text-3xl font-black text-amber-400">4.2h</p>
        </div>
    </div>

    <div class="bg-slate-900 rounded-2xl border border-slate-800 overflow-hidden">
        <table class="w-full text-left">
            <thead class="bg-slate-800 text-slate-400 text-xs uppercase">
                <tr>
                    <th class="p-4">Lead</th>
                    <th class="p-4">Etapa</th>
                    <th class="p-4">Prob. de Fechamento</th>
                    <th class="p-4">Última Atividade</th>
                </tr>
            </thead>
            <tbody class="text-sm">
                <tr class="border-b border-slate-800">
                    <td class="p-4 font-semibold">Lorena (Imobiliária)</td>
                    <td class="p-4 text-emerald-400">Fechamento</td>
                    <td class="p-4">95%</td>
                    <td class="p-4">Hoje</td>
                </tr>
                <tr class="border-b border-slate-800">
                    <td class="p-4 font-semibold">Rodrigo (CEO)</td>
                    <td class="p-4 text-blue-400">Atendimento</td>
                    <td class="p-4">70%</td>
                    <td class="p-4">Hoje</td>
                </tr>
            </tbody>
        </table>
    </div>
</body>
</html>
