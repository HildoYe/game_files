# Archaeological Sites
# -----------------------
#
# site_type_name = {				# Key of the site, used for name lookup etc.
#	picture = <sprite key>		# GFX_* sprite key for the sites image
#	desc = <triggered event desc>	# Description generator for the site, with scope this=archaeological site.
#	max_instances = <int>			# Max instances of this type a galaxy can have, only checked when using 'create_archaeological_site = random'
#	weight = <scriptable value>		# Weight used for random weight, only used when using 'create_archaeological_site = random'. scriptable value type is defined either by '<int>' or '<mean time to happen>'.
#	stages = <int>					# Should match number of defined stages below.
#	potential = <trigger>			# Trigger checking if a scope with this=fleet,from=archaeological site is potential to excavate (this will add/remove this option without giving the player a reason).
#	allow = <trigger>				# Trigger checking if a scope with this=fleet,from=archaeological site is allowed to excavate (this will toggle enable/disabled mode on buttons etc).
#	visible = <trigger>				# Trigger that checks if a scope with this=country can see the from=archaeological site
#	stage = {						# Stage definition, order dependent.
#		difficulty = <interval int>	# min max interval type. interval is defined either by '<int>' or '{ min = <int> max = <int> }' where the later will randomize a value between min and max.
#		icon = <string>				# rune icon gfx type.
#		event = <string>			# event to fire when the stage has been completed.
#	}
#	stage = {...}					# Second stage, the total number of 'stage' entries should match value of 'stages'
#	on_roll_failed = <effect>			# Effect to fire when a roll fails, with scope this=fleet, from=archaeological site.
#	on_create = <effect>			# Effect to fire upon site creation, with scope this=archaeological site.
#	on_visible = <effect>			# Effect to fire upon site visible, with scope this=country, from=archaeological site.
#}
