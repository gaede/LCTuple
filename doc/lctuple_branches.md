# Branches and variables in LCTuple


## EventBranches

- filled in [EventBranches.cc](https://github.com/iLCSoft/LCTuple/blob/master/src/EventBranches.cc#L37-L53)
- from [LCEvent.h](https://github.com/iLCSoft/LCIO/blob/master/src/cpp/include/pre-generated/EVENT/LCEvent.h)

| variable       | content/comment                                         |
|----------------|---------------------------------------------------------|
| evevt/I        | LCEvent::getEventNumber()							   |
| evrun/I        | LCEvent::getRunNumber()								   |
| evwgt/F        | LCEvent::getWeight()                                    |
| evtim/L        | LCEvent::getTimeStamp()								   |
| evsig/F        | LCEvent::getParameters().getFloatVal("CrossSection_fb") |
| evene/F        | LCEvent::getParameters().getFloatVal("Energy")          |
| evpoe/F        | LCEvent::getParameters().getFloatVal("Pol_em")          |
| evpop/F        | LCEvent::getParameters().getFloatVal("Pol_ep")          |
| evnch/I        | *number of characters in evpro*                         |
| evpro[evnch]/C | LCEvent::getParameters().getStringVal("Process")		   |


## MCParticleBranches


| variable      | content/comment                                         |
|---------------|---------------------------------------------------------|
| nmcp/I        | *number of MCParticles*                                 |
| mcori[nmcp]/I | *ID of original collection from MergeCollections.cc*    |
| mcpdg[nmcp]/I | `MCParticle::getPDG()`    |		
| mcgst[nmcp]/I | MCParticle::getGeneratorStatus()    |	
| mcsst[nmcp]/I | MCParticle::getSimulatorStatus()    |	
| mcvtx[nmcp]/F | MCParticle::getVertex()[0]    |		
| mcvty[nmcp]/F | MCParticle::getVertex()[1]    |		
| mcvtz[nmcp]/F | MCParticle::getVertex()[2]    |		
| mcepx[nmcp]/F | MCParticle::getEndpoint()[0]    |	
| mcepy[nmcp]/F | MCParticle::getEndpoint()[1]    |	
| mcepz[nmcp]/F | MCParticle::getEndpoint()[2]    |	
| mcmox[nmcp]/F | MCParticle::getMomentum()[0]    |	
| mcmoy[nmcp]/F | MCParticle::getMomentum()[1]    |	
| mcmoz[nmcp]/F | MCParticle::getMomentum()[2]    |	
| mcmas[nmcp]/F | MCParticle::getMass()    |		
| mcene[nmcp]/F | MCParticle::getEnergy()    |		
| mccha[nmcp]/F | MCParticle::getCharge()    |		
| mctim[nmcp]/F | MCParticle::getTime()    |		
| mcspx[nmcp]/F | MCParticle::getSpin()[0]    |		
| mcspy[nmcp]/F | MCParticle::getSpin()[1]    |		
| mcspz[nmcp]/F | MCParticle::getSpin()[2]    |		
| mccf0[nmcp]/I | MCParticle::getColorFlow()[0]    |	
| mccf1[nmcp]/I | MCParticle::getColorFlow()[1]    |
| mcpa0[nmcp]/I |  *index of 1. parent particle*  |
| mcpa1[nmcp]/I |  *index of 2. parent particle*  |
| mcda0[nmcp]/I |  *index of 1. daughter particle*  |
| mcda1[nmcp]/I |  *index of 2. daughter particle*  |
| mcda2[nmcp]/I |  *index of 3. daughter particle*  |
| mcda3[nmcp]/I |  *index of 4. daughter particle*  |
| mcda4[nmcp]/I |  *index of 5. daughter particle*  | 
