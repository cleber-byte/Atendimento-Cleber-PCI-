import React from 'react';
import { BarChart3, PhoneCall, Calendar, Users, AlertCircle, CheckCircle2, Clock, Snowman } from 'lucide-react';

export default function CloserDashboard() {
  const metricas = {
    contatoInicial: 7,
    atendimento: 4,
    agendamento: 2,
    reunioesRealizadas: 4
  };

  const leadsQuentes = [
    {
      id: 1,
      nome: "Rodrigo Bueno",
      etapa: "Fechamento Urgente",
      prioridade: "MÁXIMA",
      detalhes: "Contrato gerado (10k entrada + 20k boleto). Aguardando assinatura e Pix hoje.",
      corPrioridade: "bg-emerald-500/10 text-emerald-400 border-emerald-500/20",
      icon: <CheckCircle2 className="w-5 h-5 text-emerald-400" />
    },
    {
      id: 2,
      nome: "Tatiana - Tamar Imóveis",
      etapa: "Aguardando Resposta",
      prioridade: "MÁXIMA",
      detalhes: "Deu o 'sim'. Fechou ontem de apresentar ao marido. Cobrar veredito hoje.",
      corPrioridade: "bg-emerald-500/10 text-emerald-400 border-emerald-500/20",
      icon: <CheckCircle2 className="w-5 h-5 text-emerald-400" />
    },
    {
      id: 3,
      nome: "Gustavo",
      etapa: "Negociação Entrada",
      prioridade: "ALTA",
      detalhes: "Sócio Paulo travou a entrada do boleto. Aplicar script de parcelamento da entrada.",
      corPrioridade: "bg-amber-500/10 text-amber-400 border-amber-500/20",
      icon: <AlertCircle className="w-5 h-5 text-amber-400" />
    },
    {
      id: 4,
      nome: "Luciana (Sorocaba)",
      etapa: "Reunião Agendada",
      prioridade: "MÉDIA",
      detalhes: "Alinhamento estratégico com o sócio/marido Marco. Segunda (13/07) às 16:00h.",
      corPrioridade: "bg-indigo-500/10 text-indigo-400 border-indigo-500/20",
      icon: <Calendar className="w-5 h-5 text-indigo-400" />
    },
    {
      id: 5,
      nome: "Alex",
      etapa: "Reunião Agendada",
      prioridade: "MÉDIA",
      detalhes: "Confirmado com a esposa na mesa. Terça-feira (14/07) às 10:00h. Pré-call dia 13.",
      corPrioridade: "bg-indigo-500/10 text-indigo-400 border-indigo-500/20",
      icon: <Calendar className="w-5 h-5 text-indigo-400" />
    },
    {
      id: 6,
      nome: "Leonardo",
      etapa: "No Gelo (Vácuo)",
      prioridade: "BAIXA",
      detalhes: "Ofertado Pocket (12k). Sumiu e pediu 15 dias de prazo. Não demonstrar desespero.",
      corPrioridade: "bg-slate-500/10 text-slate-400 border-slate-500/20",
      icon: <Clock className="w-5 h-5 text-slate-400" />
    }
  ];

  return (
    <div className="min-h-screen bg-slate-950 text-slate-100 p-6 font-sans">
      {/* HEADER */}
      <div className="flex flex-col md:flex-row md:items-center md:justify-between border-b border-slate-800 pb-6 mb-8">
        <div>
          <h1 className="text-2xl font-bold tracking-tight text-white flex items-center gap-2">
            <BarChart3 className="text-indigo-500 w-7 h-7" /> Control Room — Cleber Solar
          </h1>
          <p className="text-sm text-slate-400 mt-1">Gestão de Performance Comercial & Pipeline PCI</p>
        </div>
        <div className="mt-4 md:mt-0 bg-slate-900 border border-slate-800 px-4 py-2 rounded-lg text-xs font-mono text-indigo-400">
          Data do Sistema: 09/07/2026
        </div>
      </div>

      {/* RIGA DE KPIS (ESTILO POWER BI) */}
      <div className="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-4 gap-4 mb-8">
        <div className="bg-slate-900 border border-slate-800 rounded-xl p-5 flex items-center justify-between shadow-lg shadow-black/20">
          <div>
            <p className="text-xs font-semibold uppercase tracking-wider text-slate-400">Contato Inicial</p>
            <h3 className="text-3xl font-bold mt-1 text-white">{metricas.contatoInicial}</h3>
          </div>
          <div className="p-3 bg-slate-800 rounded-lg text-slate-400"><PhoneCall className="w-6 h-6" /></div>
        </div>

        <div className="bg-slate-900 border border-slate-800 rounded-xl p-5 flex items-center justify-between shadow-lg shadow-black/20">
          <div>
            <p className="text-xs font-semibold uppercase tracking-wider text-slate-400">Atendimentos Ativos</p>
            <h3 className="text-3xl font-bold mt-1 text-white">{metricas.atendimento}</h3>
          </div>
          <div className="p-3 bg-slate-800 rounded-lg text-indigo-400"><Users className="w-6 h-6" /></div>
        </div>

        <div className="bg-slate-900 border border-slate-800 rounded-xl p-5 flex items-center justify-between shadow-lg shadow-black/20">
          <div>
            <p className="text-xs font-semibold uppercase tracking-wider text-slate-400">Agendamentos</p>
            <h3 className="text-3xl font-bold mt-1 text-white">{metricas.agendamento}</h3>
          </div>
          <div className="p-3 bg-slate-800 rounded-lg text-sky-400"><Calendar className="w-6 h-6" /></div>
        </div>

        <div className="bg-slate-900 border border-slate-800 rounded-xl p-5 flex items-center justify-between shadow-lg shadow-black/20">
          <div>
            <p className="text-xs font-semibold uppercase tracking-wider text-slate-400">Reuniões Feitas</p>
            <h3 className="text-3xl font-bold mt-1 text-emerald-400">{metricas.reunioesRealizadas}</h3>
          </div>
          <div className="p-3 bg-slate-800 rounded-lg text-emerald-400"><BarChart3 className="w-6 h-6" /></div>
        </div>
      </div>

      {/* PIPELINE DE ATENDIMENTOS QUENTES */}
      <div className="bg-slate-900 border border-slate-800 rounded-xl shadow-xl overflow-hidden">
        <div className="px-6 py-4 border-b border-slate-800 bg-slate-900/50 flex justify-between items-center">
          <h2 className="text-lg font-bold text-white tracking-tight">Esteira Crítica de Negociação</h2>
          <span className="text-xs font-medium px-2.5 py-1 rounded-full bg-indigo-500/10 text-indigo-400 border border-indigo-500/20">Foco Total em Recebimento</span>
        </div>
        <div className="divide-y divide-slate-800">
          {leadsQuentes.map((lead) => (
            <div key={lead.id} className="p-6 hover:bg-slate-850 transition duration-150 flex flex-col lg:flex-row lg:items-center lg:justify-between gap-4">
              <div className="flex items-start gap-4">
                <div className="mt-1 p-2 bg-slate-800 rounded-lg shrink-0">
                  {lead.icon}
                </div>
                <div>
                  <div className="flex items-center gap-3 flex-wrap">
                    <h4 className="text-base font-bold text-white">{lead.nome}</h4>
                    <span className="text-xs px-2.5 py-0.5 rounded-md font-mono bg-slate-800 text-slate-300 border border-slate-700">
                      {lead.etapa}
                    </span>
                    <span className={`text-[10px] font-bold px-2 py-0.5 rounded border ${lead.corPrioridade}`}>
                      {lead.prioridade}
                    </span>
                  </div>
                  <p className="text-sm text-slate-400 mt-2 max-w-3xl leading-relaxed">
                    {lead.detalhes}
                  </p>
                </div>
              </div>
              <div className="lg:text-right shrink-0">
                {lead.prioridade === "MÁXIMA" && (
                  <span className="inline-flex items-center gap-1.5 text-xs font-bold px-3 py-1.5 rounded-lg bg-emerald-500 text-slate-950 animate-pulse">
                    🚀 Fechar Hoje
                  </span>
                )}
                {lead.prioridade === "ALTA" && (
                  <span className="inline-flex items-center gap-1.5 text-xs font-semibold px-3 py-1.5 rounded-lg bg-amber-500 text-slate-950">
                    ⚡ Quebrar Objeção
                  </span>
                )}
                {lead.prioridade === "MÉDIA" && (
                  <span className="inline-flex items-center gap-1.5 text-xs font-medium px-3 py-1.5 rounded-lg bg-slate-800 text-slate-300 border border-slate-700">
                    🗓️ Cadenciado
                  </span>
                )}
                {lead.prioridade === "BAIXA" && (
                  <span className="inline-flex items-center gap-1.5 text-xs font-medium px-3 py-1.5 rounded-lg bg-slate-950 text-slate-500 border border-slate-900">
                    🧊 Aguardar
                  </span>
                )}
              </div>
            </div>
          ))}
        </div>
      </div>
    </div>
  );
}
