<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Dashboard de Atendimento - Cleber</title>
    <script src="https://cdn.tailwindcss.com"></script>
</head>
<body class="min-h-screen bg-gray-950 text-white p-6 font-sans">

    <div class="flex flex-col md:flex-row justify-between items-start md:items-center mb-8 border-b border-gray-800 pb-6">
        <div>
            <h1 class="text-3xl font-bold tracking-tight bg-gradient-to-r from-orange-500 to-amber-400 bg-clip-text text-transparent">
                SISTEMA DE CADÊNCIA OPERACIONAL
            </h1>
            <p class="text-gray-400 mt-1 text-sm">Performance de Atendimento — Consultor Cleber Michel</p>
        </div>
        <div class="bg-gray-900 border border-gray-800 px-4 py-2 rounded-lg mt-4 md:mt-0">
            <span class="text-xs text-gray-500 block uppercase">Atualizado em</span>
            <span class="text-sm font-semibold text-orange-400">18 de Junho, 2026</span>
        </div>
    </div>

    <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-4 gap-4 mb-8">
        <div class="bg-gray-900 border border-gray-800 p-5 rounded-xl">
            <p class="text-xs text-gray-400 uppercase font-medium">Total em Carteira</p>
            <p class="text-3xl font-bold mt-2 text-white">49 <span class="text-sm font-normal text-gray-500">leads</span></p>
        </div>
        <div class="bg-gray-900 border border-gray-800 p-5 rounded-xl border-l-4 border-l-emerald-500">
            <p class="text-xs text-emerald-400 uppercase font-medium">Ganhos Pagos</p>
            <p class="text-3xl font-bold mt-2 text-emerald-400">4 <span class="text-sm font-normal text-gray-500">fechados</span></p>
        </div>
        <div class="bg-gray-900 border border-gray-800 p-5 rounded-xl border-l-4 border-l-amber-500">
            <p class="text-xs text-amber-400 uppercase font-medium">Em Atendimento Ativo</p>
            <p class="text-3xl font-bold mt-2 text-amber-400">28 <span class="text-sm font-normal text-gray-500">no funil</span></p>
        </div>
        <div class="bg-gray-900 border border-gray-800 p-5 rounded-xl border-l-4 border-l-blue-500">
            <p class="text-xs text-blue-400 uppercase font-medium">Contato Inicial (Triagem)</p>
            <p class="text-3xl font-bold mt-2 text-blue-400">21 <span class="text-sm font-normal text-gray-500">novos</span></p>
        </div>
    </div>

    <div class="bg-gray-900 border border-gray-800 p-6 rounded-xl mb-8">
        <h3 class="text-lg font-bold mb-4 text-gray-200">Distribuição Operacional por Origem do Lead</h3>
        <div class="space-y-4">
            <div>
                <div class="flex justify-between text-xs mb-1">
                    <span class="text-gray-300 font-medium">Planilha Pedro / Comercial</span>
                    <span class="text-orange-400 font-bold">3 Atendimentos (Ganhos)</span>
                </div>
                <div class="w-full bg-gray-800 h-3 rounded-full overflow-hidden">
                    <div class="bg-gradient-to-r from-orange-500 to-amber-400 h-full w-[45%]"></div>
                </div>
            </div>
            <div>
                <div class="flex justify-between text-xs mb-1">
                    <span class="text-gray-300 font-medium">Campanha JOKER</span>
                    <span class="text-orange-400 font-bold">1 Atendimento (PCI Ganho)</span>
                </div>
                <div class="w-full bg-gray-800 h-3 rounded-full overflow-hidden">
                    <div class="bg-gradient-to-r from-orange-500 to-amber-400 h-full w-[20%]"></div>
                </div>
            </div>
            <div>
                <div class="flex justify-between text-xs mb-1">
                    <span class="text-gray-300 font-medium">Inbound Site / Landing Page / Redes</span>
                    <span class="text-orange-400 font-bold">45 Atendimentos</span>
                </div>
                <div class="w-full bg-gray-800 h-3 rounded-full overflow-hidden">
                    <div class="bg-gradient-to-r from-orange-500 to-amber-400 h-full w-[85%]"></div>
                </div>
            </div>
        </div>
    </div>

    <div class="bg-gray-900 border border-gray-800 rounded-xl overflow-hidden">
        <div class="p-6 border-b border-gray-800">
            <h3 class="text-lg font-bold text-gray-200">Painel de Controle de Leads e Cadência</h3>
        </div>
        <div class="overflow-x-auto">
            <table class="w-full text-left border-collapse">
                <thead>
                    <tr class="bg-gray-950 text-gray-400 text-xs uppercase font-semibold border-b border-gray-800">
                        <th class="p-4">Nome do Lead</th>
                        <th class="p-4">Produto</th>
                        <th class="p-4">Origem do Lead</th>
                        <th class="p-4">Status</th>
                        <th class="p-4 text-center">Dias Sem Contato</th>
                    </tr>
                </thead>
                <tbody class="divide-y divide-gray-800 text-sm text-gray-300">
                    <tr class="hover:bg-gray-900/50 transition-colors">
                        <td class="p-4 font-semibold text-white">Guilherme Zaggia</td>
                        <td class="p-4"><span class="px-2 py-1 rounded text-xs font-bold bg-purple-950 text-purple-300 border border-purple-800">PCI</span></td>
                        <td class="p-4 font-medium">Campanha JOKER</td>
                        <td class="p-4"><span class="px-2.5 py-0.5 rounded-full text-xs font-semibold bg-emerald-950 text-emerald-400 border border-emerald-800">Ganho</span></td>
                        <td class="p-4 text-center font-bold text-gray-400">0d</td>
                    </tr>
                    <tr class="hover:bg-gray-900/50 transition-colors">
                        <td class="p-4 font-semibold text-white">Rodrigo</td>
                        <td class="p-4"><span class="px-2 py-1 rounded text-xs font-bold bg-cyan-950 text-cyan-300 border border-cyan-800">Líder</span></td>
                        <td class="p-4 font-medium">Planilha Pedro</td>
                        <td class="p-4"><span class="px-2.5 py-0.5 rounded-full text-xs font-semibold bg-emerald-950 text-emerald-400 border border-emerald-800">Ganho</span></td>
                        <td class="p-4 text-center font-bold text-gray-400">0d</td>
                    </tr>
                    <tr class="hover:bg-gray-900/50 transition-colors">
                        <td class="p-4 font-semibold text-white">Bethania</td>
                        <td class="p-4"><span class="px-2 py-1 rounded text-xs font-bold bg-cyan-950 text-cyan-300 border border-cyan-800">Líder</span></td>
                        <td class="p-4 font-medium">Planilha Pedro</td>
                        <td class="p-4"><span class="px-2.5 py-0.5 rounded-full text-xs font-semibold bg-emerald-950 text-emerald-400 border border-emerald-800">Ganho</span></td>
                        <td class="p-4 text-center font-bold text-gray-400">0d</td>
                    </tr>
                    <tr class="hover:bg-gray-900/50 transition-colors">
                        <td class="p-4 font-semibold text-white">Shimilly</td>
                        <td class="p-4"><span class="px-2 py-1 rounded text-xs font-bold bg-purple-950 text-purple-300 border border-purple-800">PCI</span></td>
                        <td class="p-4 font-medium">Planilha Pedro</td>
                        <td class="p-4"><span class="px-2.5 py-0.5 rounded-full text-xs font-semibold bg-emerald-950 text-emerald-400 border border-emerald-800">Ganho</span></td>
                        <td class="p-4 text-center font-bold text-gray-400">0d</td>
                    </tr>
                    <tr class="hover:bg-gray-900/50 transition-colors">
                        <td class="p-4 font-semibold text-white">Ricardo</td>
                        <td class="p-4"><span class="px-2 py-1 rounded text-xs font-bold bg-purple-950 text-purple-300 border border-purple-800">PCI</span></td>
                        <td class="p-4 font-medium">Site (Londrina)</td>
                        <td class="p-4"><span class="px-2.5 py-0.5 rounded-full text-xs font-semibold bg-amber-950 text-amber-400 border border-amber-800">Atendimento</span></td>
                        <td class="p-4 text-center font-bold text-gray-400">0d</td>
                    </tr>
                    <tr class="hover:bg-gray-900/50 transition-colors">
                        <td class="p-4 font-semibold text-white">Luiz</td>
                        <td class="p-4"><span class="px-2 py-1 rounded text-xs font-bold bg-cyan-950 text-cyan-300 border border-cyan-800">Líder</span></td>
                        <td class="p-4 font-medium">Base Ativa</td>
                        <td class="p-4"><span class="px-2.5 py-0.5 rounded-full text-xs font-semibold bg-amber-950 text-amber-400 border border-amber-800">Atendimento</span></td>
                        <td class="p-4 text-center font-bold text-gray-400">1d</td>
                    </tr>
                    <tr class="hover:bg-gray-900/50 transition-colors">
                        <td class="p-4 font-semibold text-white">Gilmara</td>
                        <td class="p-4"><span class="px-2 py-1 rounded text-xs font-bold bg-cyan-950 text-cyan-300 border border-cyan-800">Líder</span></td>
                        <td class="p-4 font-medium">Formulário Interesse</td>
                        <td class="p-4"><span class="px-2.5 py-0.5 rounded-full text-xs font-semibold bg-amber-950 text-amber-400 border border-amber-800">Atendimento</span></td>
                        <td class="p-4 text-center font-bold text-gray-400">1d</td>
                    </tr>
                    <tr class="hover:bg-gray-900/50 transition-colors">
                        <td class="p-4 font-semibold text-white">Milena</td>
                        <td class="p-4"><span class="px-2 py-1 rounded text-xs font-bold bg-cyan-950 text-cyan-300 border border-cyan-800">Líder</span></td>
                        <td class="p-4 font-medium">Formulário Interesse</td>
                        <td class="p-4"><span class="px-2.5 py-0.5 rounded-full text-xs font-semibold bg-amber-950 text-amber-400 border border-amber-800">Atendimento</span></td>
                        <td class="p-4 text-center font-bold text-gray-400">2d</td>
                    </tr>
                    <tr class="hover:bg-gray-900/50 transition-colors">
                        <td class="p-4 font-semibold text-white">Jan Guimaraes</td>
                        <td class="p-4"><span class="px-2 py-1 rounded text-xs font-bold bg-purple-950 text-purple-300 border border-purple-800">PCI</span></td>
                        <td class="p-4 font-medium">Mapear</td>
                        <td class="p-4"><span class="px-2.5 py-0.5 rounded-full text-xs font-semibold bg-blue-950 text-blue-400 border border-blue-800">Contato Inicial</span></td>
                        <td class="p-4 text-center font-bold text-gray-400">0d</td>
                    </tr>
                    <tr class="hover:bg-gray-900/50 transition-colors">
                        <td class="p-4 font-semibold text-white">Fabiano</td>
                        <td class="p-4"><span class="px-2 py-1 rounded text-xs font-bold bg-cyan-950 text-cyan-300 border border-cyan-800">Líder</span></td>
                        <td class="p-4 font-medium">Mapear</td>
                        <td class="p-4"><span class="px-2.5 py-0.5 rounded-full text-xs font-semibold bg-blue-950 text-blue-400 border border-blue-800">Contato Inicial</span></td>
                        <td class="p-4 text-center font-bold text-gray-400">0d</td>
                    </tr>
                    <tr class="hover:bg-gray-900/50 transition-colors">
                        <td class="p-4 font-semibold text-white">Laira Stephane</td>
                        <td class="p-4"><span class="px-2 py-1 rounded text-xs font-bold bg-cyan-950 text-cyan-300 border border-cyan-800">Líder</span></td>
                        <td class="p-4 font-medium">Landing Page</td>
                        <td class="p-4"><span class="px-2.5 py-0.5 rounded-full text-xs font-semibold bg-blue-950 text-blue-400 border border-blue-800">Contato Inicial</span></td>
                        <td class="p-4 text-center font-bold text-gray-400">1d</td>
                    </tr>
                </tbody>
            </table>
        </div>
    </div>
</body>
</html>
