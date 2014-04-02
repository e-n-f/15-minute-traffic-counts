all: walk-rank turn-rank

turn: ../*.csv get-turn
	./get-turn ../*.csv > turn

walk-rank: turn
	sort -rn turn | awk '{print NR, $$0}' > walk-rank

turn-rank: turn
	sort -rn -k2 turn | awk '{print NR, $$0}' > turn-rank
