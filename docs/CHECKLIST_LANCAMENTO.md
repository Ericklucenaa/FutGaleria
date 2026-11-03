# Checklist antes de publicar a primeira Release

- [ ] Servidor de licenças configurado com HTTPS e banco persistente/backups.
- [ ] Checkout real configurado e aprovação do processador de pagamentos.
- [ ] Compra e revogação de licença testadas de ponta a ponta.
- [ ] Links e preços coerentes nos três idiomas.
- [ ] Termos de uso, privacidade e suporte efetivamente publicados.
- [ ] Riscos da automação avaliados diante das regras da EA.
- [ ] Revisão de segurança concluída.
- [ ] `python -m pytest -q extension/tests server/tests` passou no repositório privado.
- [ ] `python scripts/pack_release.py` gerou ZIP e hash após validar URLs.
- [ ] `python scripts/audit_public_repo.py ...` não encontrou código no repositório público.
- [ ] Instalação em perfil limpo do Chrome conferida.
- [ ] Apenas ZIP e hash publicados como assets da Release (não como arquivos git).
