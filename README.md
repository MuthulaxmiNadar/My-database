# AIRFORCE DBMS

#Entity Sets

officer (officer _id, officer _name, officer_contact height,weight)

weapons (weapon_id, weapon_name, type, mode) 

command(command_name, headquarter)

war(war_name ,war_year)

award(award_name, awarding_year)

Two officer entity sets:  airmen and health_officer
	common attribute - officer _id
	airmen(rank, sector)
	health_officer (specialization)
  
  
#Relationship Sets

belongs  1:N command with officer, both total

uses M:N airmen with weapons, airmen partial, weapons total

participates M:N airmen with war airmen total, war partial

is awarded  M:N officers with award, officers total, reward partial


#Relational Model-Schema

officer (officer _id, officer _name, officer_contact, height, weight, c_name*)

weapons (weapon_id, weapon_name, type, mode)

command(command_name, headquarter)

war(war_name ,war_year)

award(award_name, awarding_year)

participates(officer_id*, war_name*)

is rewarded(officer_id* ,award_name*)

uses(officer_id* ,weapon_id*)

airmen(officer_id, rank, sector)

health_officer (officer_id, specialization)






	
	
		
	







