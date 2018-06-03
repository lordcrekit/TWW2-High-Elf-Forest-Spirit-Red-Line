##
# Mod README.
#
# Insertions are described on lines starting and ending with "!!!!"
# Changes are described on lines starting and ending with "????"
# Deletions are described on lines starting and ending with "----"
# All other lines are existing values shown for reference, as to describe why changes were made as stated.
##

data.pack	
	##
	# Here are the character abilities. We are looking at this for reference.
	##
	??????????
		wh2_main_effect_skill_melee_attack_increase_hef_spears_seaguard_archers
		wh2_main_effect_skill_melee_defence_increase_hef_spears_seaguard_archers
		wh2_main_effect_tech_melee_attack_increase_hef_swordmasters_lions_phoenixg
		wh2_main_effect_tech_melee_defence_increase_hef_swordmasters_lions_phoenixg

	##
	# Here are where buffs are assigned to unit sets
	##
	effect_bonus_value_ids_unit_sets_tables
		wh2_main_effect_skill_melee_attack_increase_hef_spears_seaguard_archers		hef_archers
		wh2_main_effect_skill_melee_attack_increase_hef_spears_seaguard_archers		hef_seaguard
		wh2_main_effect_skill_melee_attack_increase_hef_spears_seaguard_archers		hef_spearmen
!!!!		wh2_main_effect_skill_melee_attack_increase_hef_spears_seaguard_archers		lordcrekit_hef_dryads	!!!!

		wh2_main_effect_skill_melee_defence_increase_hef_spears_seaguard_archers	hef_archers
		wh2_main_effect_skill_melee_defence_increase_hef_spears_seaguard_archers	hef_seaguard
		wh2_main_effect_skill_melee_defence_increase_hef_spears_seaguard_archers	hef_spearmen
!!!!		wh2_main_effect_skill_melee_defence_increase_hef_spears_seaguard_archers	lordcrekit_hef_dryads	!!!!

		wh2_main_effect_tech_melee_attack_increase_hef_swordmasters_lions_phoenixg	hef_phoenixguard
		wh2_main_effect_tech_melee_attack_increase_hef_swordmasters_lions_phoenixg	hef_swordmasters
		wh2_main_effect_tech_melee_attack_increase_hef_swordmasters_lions_phoenixg	hef_whitelions
!!!!		wh2_main_effect_tech_melee_attack_increase_hef_swordmasters_lions_phoenixg	lordcrekit_hef_treekin	!!!!

		wh2_main_effect_tech_melee_defence_increase_hef_swordmasters_lions_phoenixg	hef_phoenixguard
		wh2_main_effect_tech_melee_defence_increase_hef_swordmasters_lions_phoenixg	hef_swordmasters
		wh2_main_effect_tech_melee_defence_increase_hef_swordmasters_lions_phoenixg	hef_whitelions
!!!!		wh2_main_effect_tech_melee_defence_increase_hef_swordmasters_lions_phoenixg	lordcrekit_hef_treekin	!!!!

	##
	# Here are where the unit sets are defind
	##
	unit_sets_tables
		hef_archers			false	-1	-1
		hef_seaguard			false	-1	-1
		hef_spearmen			false	-1	-1
		hef_archer_seaguard_rank7	false	7	9
!!!!		lordcrekit_hef_dryads		false	-1	-1		!!!!

		hef_phoenixguard		false	-1	-1
		hef_swordmasters		false	-1	-1
		hef_whitelions			false	-1	-1
!!!!		lordcrekit_hef_treekin		false	-1	-1		!!!!

!!!!		lordcrekit_hef_treeman		false	-1	-1		!!!!

	##
	# Here are where we bind units to unit sets
	##
	unit_set_to_unit_junctions_tables
		null	null	null	wh2_main_hef_inf_archers_0		hef_archers			False
		null	null	null	wh2_main_hef_inf_archers_1		hef_archers			False

		null	null	null	wh2_main_hef_inf_archers_0		hef_archer_seaguard_rank7	False
		null	null	null	wh2_main_hef_inf_archers_1		hef_archer_seaguard_rank7	False
		null	null	null	wh2_main_hef_inf_lothern_sea_guard_0	hef_archer_seaguard_rank7	False
		null	null	null	wh2_main_hef_inf_lothern_sea_guard_1	hef_archer_seaguard_rank7	False

!!!!		null	null	null	wh2_dlc10_hef_inf_dryads_0		lordcrekit_hef_dryads		False		!!!!
!!!!		null	null	null	wh2_dlc10_hef_mon_treekin_0		lordcrekit_hef_treekin		False		!!!!
!!!!		null	null	null	wh2_dlc10_hef_mon_treeman_0		lordcrekit_hef_treeman		False		!!!!

	##
	# Here are where the units are
	##
	land_unit_tables
		# Units already in sets
		wh2_main_hef_inf_archers_0
		wh2_main_hef_inf_archers_1
		wh2_main_hef_inf_lothern_sea_guard_0
		wh2_main_hef_inf_lothern_sea_guard_1
		wh2_main_hef_inf_spearmen_0
		
		# These are the units we want to ad to our new sets.
		wh2_dlc10_hef_inf_dryads_0
		wh2_dlc10_hef_mon_treekin_0
		wh2_dlc10_hef_mon_treeman_0

		# The actual wood elf units for reference.
		wh_dlc05_wef_inf_dryads_0
		wh_dlc05_wef_mon_treekin_0
		wh_dlc05_wef_mon_treeman_0
